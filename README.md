<html><head><base href="https://camiloduvane.github.io/Funcionarios/">
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
<a href="https://camiloduvane.github.io/DMTT/" class="back-button">← Voltar</a>

<div class="search-container">
    <input type="text" id="nameSearch" placeholder="Pesquisar por nome...">
    <select id="departmentSearch">
        <option value="">Todos os Departamentos</option>
        <option value="DARHF">DARHF</option>
        <option value="DL">DL</option>
        <option value="DOT">DOT</option>
        <option value="DTP">DTP</option>
        <option value="Secretária">Secretária</option>
    </select>
</div>
<table id="employeeTable">
    <thead>
        <tr>
            <th>Foto</th>
            <th>Nome</th>
            <th>Função</th>
            <th>Departamento</th>
            <th>Contacto</th>
            <th>Email</th>
            <th>Status</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td><svg class="employee-photo" viewBox="0 0 50 50">
                <circle cx="25" cy="20" r="15" fill="#51cf66"/>
                <circle cx="25" cy="55" r="25" fill="#51cf66"/>
            </svg></td>
            <td>Camilo Wiliamo Duvane</td>
            <td>Analista é desenvolvedor de sistemas de gestão, Auditoria e Financeiro</td>
            <td>DL</td>
            <td>+258 84 247 9404</td>
            <td>camilowilliam0@gmail.com</td>
            <td class="status-active">Activo</td>
        </tr>
        <tr>
            <td><svg class="employee-photo" viewBox="0 0 50 50">
                <circle cx="25" cy="20" r="15" fill="#007bff"/>
                <circle cx="25" cy="55" r="25" fill="#007bff"/>
            </svg></td>
            <td>Fernando Uache</td>
            <td>Gestor Sénior</td>
            <td>Vereador</td>
            <td>+258 84 123 4567</td>
            <td>fernando.uache@camiloduvane.com</td>
            <td class="status-active">Activo</td>
        </tr>
        <tr>
            <td><svg class="employee-photo" viewBox="0 0 50 50">
                <circle cx="25" cy="20" r="15" fill="#ff6b6b"/>
                <circle cx="25" cy="55" r="25" fill="#ff6b6b"/>
            </svg></td>
            <td>Nelson Gustavo Massango</td>
            <td>Gestor Sénior</td>
            <td>DMTT</td>
            <td>+258 85 234 5678</td>
            <td>nelson.massango@camiloduvane.com</td>
            <td class="status-active">Activo</td>
        </tr>
        <tr>
            <td><svg class="employee-photo" viewBox="0 0 50 50">
                <circle cx="25" cy="20" r="15" fill="#51cf66"/>
                <circle cx="25" cy="55" r="25" fill="#51cf66"/>
            </svg></td>
            <td>Carlos Vilanculos</td>
            <td>Analista Financeiro</td>
            <td>DARHF</td>
            <td>+258 86 345 6789</td>
            <td>carlos.vilanculos@camiloduvane.com</td>
            <td class="status-active">Activo</td>
        </tr>
        <tr>
          <td><svg class="employee-photo" viewBox="0 0 50 50">
                <circle cx="25" cy="20" r="15" fill="#51cf66"/>
                <circle cx="25" cy="55" r="25" fill="#51cf66"/>
            </svg></td>
            <td>Amilton Tembe</td>
            <td>Analista de Licencas</td>
            <td>DL</td>
            <td>+258 86 345 6789</td>
            <td>amilton.tembe@camiloduvane.com</td>
            <td class="status-active">Activo</td>
        </tr>
            <td><svg class="employee-photo" viewBox="0 0 50 50">
                <circle cx="25" cy="20" r="15" fill="#51cf66"/>
                <circle cx="25" cy="55" r="25" fill="#51cf66"/>
            </svg></td>
            <td>Baltazar Hilario</td>
            <td>Operações</td>
            <td>DOT</td>
            <td>+258 86 345 6789</td>
            <td>baltazar.hilario@camiloduvane.com</td>
            <td class="status-inactive">Inativo</td>
        </tr>
        <tr>
            <td><svg class="employee-photo" viewBox="0 0 50 50">
                <circle cx="25" cy="20" r="15" fill="#51cf66"/>
                <circle cx="25" cy="55" r="25" fill="#51cf66"/>
            </svg></td>
            <td>Vasco Nhaquila</td>
            <td>Relações Públicas</td>
            <td>DTP</td>
            <td>+258 86 345 6789</td>
            <td>vnhawuila@gmail.com</td>
            <td class="status-inactive">Inativo</td>
        </tr>
        <tr>
            <td><svg class="employee-photo" viewBox="0 0 50 50">
                <circle cx="25" cy="20" r="15" fill="#51cf66"/>
                <circle cx="25" cy="55" r="25" fill="#51cf66"/>
            </svg></td>
            <td>Safo Mahumana</td>
            <td>Supervisor</td>
            <td>DARHF</td>
            <td>+258 86 345 6789</td>
            <td>safomahumana@camiloduvane.com</td>
            <td class="status-inactive">Inativo</td>
        </tr>
        <tr>
            <td><svg class="employee-photo" viewBox="0 0 50 50">
                <circle cx="25" cy="20" r="15" fill="#51cf66"/>
                <circle cx="25" cy="55" r="25" fill="#51cf66"/>
            </svg></td>
            <td>José Chiau</td>
            <td>Analista de Licencas</td>
            <td>Secretária</td>
            <td>+258 86 345 6789</td>
            <td>josechiau@camiloduvane.com</td>
            <td class="status-inactive">Inativo</td>
        </tr>
        <tr>
            <td><svg class="employee-photo" viewBox="0 0 50 50">
                <circle cx="25" cy="20" r="15" fill="#51cf66"/>
                <circle cx="25" cy="55" r="25" fill="#51cf66"/>
            </svg></td>
            <td>Catarina Chiquava</td>
            <td>Analista de Licencas</td>
            <td>DOT</td>
            <td>+258 86 345 6789</td>
            <td>amilton.tembe@camiloduvane.com</td>
            <td class="status-inactive">Inativo</td>
        </tr>





        
    </tbody>
</table>
<script>
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
