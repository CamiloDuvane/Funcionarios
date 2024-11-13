<html><head><base href="https://example.com/employee-directory/">
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Lista de Funcionários</title>
<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');

body {
    font-family: 'Roboto', sans-serif;
    margin: 20px;
    background: #f5f5f5;
}

.back-button {
    background: #007bff;
    color: white;
    padding: 10px 20px;
    text-decoration: none;
    border-radius: 5px;
    display: inline-block;
    margin-bottom: 20px;
}
.search-container {
    background: white;
    padding: 20px;
    border-radius: 5px;
    margin-bottom: 20px;
    box-shadow: 0 2px 4px rgba(0,0,0,0.1);
}

.search-container input, .search-container select {
    padding: 8px;
    margin-right: 10px;
    border: 1px solid #ddd;
    border-radius: 4px;
}

table {
    width: 100%;
    border-collapse: collapse;
    background: white;
    box-shadow: 0 2px 4px rgba(0,0,0,0.1);
}

th, td {
    padding: 12px;
    text-align: left;
    border-bottom: 1px solid #ddd;
}

th {
    background-color: #007bff;
    color: white;
}

tr:hover {
    background-color: #f5f5f5;
}
.employee-photo {
    width: 50px;
    height: 50px;
    border-radius: 50%;
    object-fit: cover;
}
.status-active {
    color: green;
    font-weight: bold;
}

.status-inactive {
    color: red;
    font-weight: bold;
}
</style>
</head>
<body>
<a href="https://example.com/romantic-proposal/" class="back-button">← Voltar</a>

<div class="search-container">
    <input type="text" id="nameSearch" placeholder="Pesquisar por nome...">
    <select id="departmentSearch">
        <option value="">Todos os Departamentos</option>
        <option value="TI">TI</option>
        <option value="RH">RH</option>
        <option value="Financeiro">Financeiro</option>
        <option value="Marketing">Marketing</option>
    </select>
</div>
document.getElementById('nameSearch').addEventListener('input', filterTable);
document.getElementById('departmentSearch').addEventListener('change', filterTable);

function filterTable() {
    const nameFilter = document.getElementById('nameSearch').value.toLowerCase();
    const departmentFilter = document.getElementById('departmentSearch').value.toLowerCase();
    const rows = document.querySelectorAll('#employeeTable tbody tr');

    rows.forEach(row => {
        const name = row.children[1].textContent.toLowerCase();
        const department = row.children[3].textContent.toLowerCase();
        const matchesName = name.includes(nameFilter);
        const matchesDepartment = !departmentFilter || department === departmentFilter;
        
        row.style.display = matchesName && matchesDepartment ? '' : 'none';
    });
}
</script>
</body>
</html>
