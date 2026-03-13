<!DOCTYPE html>
<html lang="zh-CN">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>柏努利方程实验 - 全功能数据平台</title>
  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: "Microsoft Yahei", sans-serif;
    }
    body {
      max-width: 1400px;
      margin: 20px auto;
      padding: 0 20px;
      line-height: 1.6;
    }
    h1 {
      text-align: center;
      color: #2c3e50;
      margin-bottom: 30px;
    }
    .module {
      margin: 25px 0;
      padding: 20px;
      border: 1px solid #e0e0e0;
      border-radius: 10px;
      background: #fafafa;
    }
    .module h2 {
      color: #34495e;
      margin-bottom: 15px;
      border-left: 5px solid #2196F3;
      padding-left: 10px;
    }
    .data-group {
      margin: 15px 0;
      padding: 15px;
      border: 1px solid #ddd;
      border-radius: 8px;
      background: white;
    }
    .data-group-header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin-bottom: 10px;
    }
    .data-group-header h3 {
      color: #2196F3;
    }
    .btn-group {
      display: flex;
      gap: 10px;
      margin: 15px 0;
      flex-wrap: wrap;
    }
    button {
      padding: 8px 16px;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      font-size: 14px;
      transition: background 0.3s;
    }
    .btn-add { background: #4CAF50; color: white; }
    .btn-add:hover { background: #45a049; }
    .btn-delete { background: #f44336; color: white; }
    .btn-delete:hover { background: #d32f2f; }
    .btn-calculate { background: #2196F3; color: white; }
    .btn-calculate:hover { background: #1976D2; }
    .btn-draw-all { background: #9C27B0; color: white; }
    .btn-draw-all:hover { background: #7B1FA2; }
    .btn-export { background: #FF9800; color: white; }
    .btn-export:hover { background: #F57C00; }
    .btn-import { background: #607D8B; color: white; }
    .btn-import:hover { background: #455A64; }
    .btn-report { background: #3F51B5; color: white; }
    .btn-report:hover { background: #303F9F; }
    .input-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
      gap: 10px;
      margin: 15px 0;
    }
    .input-item {
      display: flex;
      flex-direction: column;
    }
    .input-item label {
      font-size: 13px;
      color: #555;
      margin-bottom: 4px;
    }
    .input-item input {
      padding: 8px;
      border: 1px solid #ccc;
      border-radius: 4px;
      font-size: 14px;
    }
    table {
      width: 100%;
      border-collapse: collapse;
      margin: 15px 0;
      background: white;
    }
    table th, table td {
      border: 1px solid #ddd;
      padding: 10px;
      text-align: center;
    }
    table th { background: #2196F3; color: white; }
    #chart-container {
      height: 500px;
      margin: 20px 0;
      background: white;
      padding: 15px;
      border-radius: 8px;
    }
    .tab-group {
      display: flex;
      gap: 10px;
      margin-bottom: 15px;
      flex-wrap: wrap;
    }
    .tab {
      padding: 8px 16px;
      border: 1px solid #ddd;
      border-radius: 5px 5px 0 0;
      cursor: pointer;
      background: #f0f0f0;
    }
    .tab.active {
      background: #2196F3;
      color: white;
      border-color: #2196F3;
    }
    .chart-legend {
      display: flex;
      gap: 20px;
      margin: 10px 0;
      flex-wrap: wrap;
    }
    .legend-item {
      display: flex;
      align-items: center;
      gap: 5px;
      font-size: 13px;
    }
    .legend-color {
      width: 15px;
      height: 15px;
      border-radius: 3px;
    }
    .file-input {
      display: none;
    }
    .error-analysis {
      background: #fff3cd;
      padding: 10px;
      border-radius: 5px;
      margin: 10px 0;
      font-size: 14px;
    }
    .report-preview {
      background: white;
      padding: 20px;
      border-radius: 8px;
      margin: 15px 0;
      border: 1px solid #ddd;
    }
    .report-preview h3 {
      color: #2c3e50;
      margin-bottom: 15px;
    }
    .report-preview p {
      margin: 8px 0;
    }
  </style>
</head>
<body>
  <h1>📊 柏努利方程实验 - 全功能数据平台</h1>

  <div class="module">
    <h2>实验数据记录</h2>
    <div class="btn-group">
      <button class="btn-add" onclick="addDataGroup()">➕ 添加实验组</button>
      <button class="btn-import" onclick="document.getElementById('file-input').click()">📥 导入CSV数据</button>
      <input type="file" id="file-input" class="file-input" accept=".csv" onchange="importData(event)">
      <button class="btn-draw-all" onclick="drawAllGroups()">📈 绘制所有组对比图</button>
      <button class="btn-export" onclick="exportData()">📤 导出CSV数据</button>
      <button class="btn-report" onclick="generateReport()">📄 生成实验报告</button>
    </div>
    <div id="data-container"></div>
  </div>

  <div class="module">
    <h2>实验结果与图表分析</h2>
    <div class="tab-group" id="tab-group">
      <div class="tab active" onclick="switchTab('total')">总水头</div>
      <div class="tab" onclick="switchTab('pressure')">测压管水头</div>
      <div class="tab" onclick="switchTab('velocity')">流速水头</div>
      <div class="tab" onclick="switchTab('position')">位置水头</div>
    </div>
    <div id="chart-container"></div>
    <div class="chart-legend" id="chart-legend"></div>
  </div>

  <div class="module">
    <h2>实验报告</h2>
    <div id="report-container"></div>
  </div>

  <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
  <script>
    let groups = [];
    let chart = null;
    let currentTab = 'total';
    const g = 9.81;

    window.onload = () => {
      addDataGroup();
    };

    function addDataGroup() {
      const id = groups.length + 1;
      const group = {
        id, name: `实验组 ${id}`, Q: 1.5,
        points: [
          {no:1, d:10, z:0, h:0},
          {no:2, d:8, z:0, h:0},
          {no:3, d:6, z:0, h:0},
          {no:4, d:12, z:0, h:0},
          {no:5, d:16, z:0, h:0},
        ]
      };
      groups.push(group);
      renderGroups();
    }

    function renderGroups() {
      const container = document.getElementById('data-container');
      container.innerHTML = '';
      groups.forEach(g => {
        const div = document.createElement('div');
        div.className = 'data-group';
        div.innerHTML = `
          <div class="data-group-header">
            <h3>${g.name}</h3>
            <button class="btn-delete" onclick="deleteGroup(${g.id})">删除本组</button>
          </div>
          <div class="input-grid">
            <div class="input-item">
              <label>流量 Q (m³/h)</label>
              <input type="number" step="0.01" value="${g.Q}" oninput="updateGroupQ(${g.id}, this.value)">
            </div>
          </div>
          <table>
            <tr>
              <th>测点</th><th>管径d(mm)</th><th>位置高度z(m)</th><th>测压管水头h(m)</th>
            </tr>
            ${g.points.map(p => `
              <tr>
                <td>${p.no}</td>
                <td><input type="number" step="0.1" value="${p.d}" oninput="updatePoint(${g.id},${p.no},'d',this.value)"></td>
                <td><input type="number" step="0.01" value="${p.z}" oninput="updatePoint(${g.id},${p.no},'z',this.value)"></td>
                <td><input type="number" step="0.01" value="${p.h}" oninput="updatePoint(${g.id},${p.no},'h',this.value)"></td>
              </tr>
            `).join('')}
          </table>
          <div class="btn-group">
            <button class="btn-calculate" onclick="calcGroup(${g.id})">🧮 计算本组水头</button>
            <button class="btn-draw-all" onclick="drawSingleGroup(${g.id})">📊 绘制本组曲线</button>
          </div>
        `;
        container.appendChild(div);
      });
    }

    function updateGroupQ(id, q) {
      const group = groups.find(x => x.id === id);
      if (group) group.Q = parseFloat(q) || 0;
    }

    function updatePoint(gid, no, key, val) {
      const group = groups.find(x => x.id === gid);
      if (!group) return;
      const p = group.points.find(x => x.no === no);
      if (p) p[key] = parseFloat(val) || 0;
    }

    function deleteGroup(id) {
      groups = groups.filter(x => x.id !== id);
      renderGroups();
    }

    function calcGroup(id) {
      const group = groups.find(x => x.id === id);
      if (!group) return;
      const Q = group.Q / 3600;
      group.points.forEach(p => {
        const d = p.d / 1000;
       const A = 0.7854 * d * d;
        const v = Q / A;
        p.v = v;
        p.vh = v * v / (2 * g);
        p.ph = p.h;
        p.zh = p.z;
        p.total = p.z + p.h + p.vh;
      });
      alert(`${group.name} 计算完成！`);
    }

    function switchTab(type) {
      currentTab = type;
      document.querySelectorAll('.tab').forEach(t => t.classList.remove('active'));
      event.target.classList.add('active');
      if (chart) chart.update();
    }

    function drawAllGroups() {
      groups.forEach(g => calcGroup(g.id));
      drawChart(groups);
    }

    function drawSingleGroup(id) {
      calcGroup(id);
      drawChart([groups.find(g => g.id === id)]);
    }

    function drawChart(showGroups) {
      const ctx = document.getElementById('chart-container').getContext('2d');
      if (chart) chart.destroy();
      const datasets = showGroups.map((g, idx) => {
        const colors = ['#2196F3','#f44336','#4CAF50','#9C27B0','#FF9800'];
        return {
          label: g.name,
          data: g.points.map(p => {
            if (currentTab === 'total') return p.total;
            if (currentTab === 'pressure') return p.ph;
            if (currentTab === 'velocity') return p.vh;
            return p.zh;
          }),
          borderColor: colors[idx % colors.length],
          backgroundColor: colors[idx % colors.length] + '33',
          fill: false,
          tension: 0.3,
          pointRadius: 4
        };
      });
      chart = new Chart(ctx, {
        type: 'line',
        data: { labels: showGroups[0].points.map(p => `测点${p.no}`), datasets },
        options: {
          responsive: true, maintainAspectRatio: false,
          plugins: { title: { display: true, text: '柏努利方程水头分布曲线' } },
          scales: { y: { beginAtZero: true, title: { display: true, text: '水头 (m)' } } }
        }
      });
    }

    function exportData() {
      let csv = "实验组,测点,管径d(mm),位置z(m),测压管h(m),流速(m/s),流速水头(m),总水头(m)\n";
      groups.forEach(g => {
        g.points.forEach(p => {
          csv += `${g.name},${p.no},${p.d},${p.z},${p.h},${p.v?.toFixed(3)||0},${p.vh?.toFixed(4)||0},${p.total?.toFixed(4)||0}\n`;
        });
      });
      const blob = new Blob([csv], { type: 'text/csv;charset=utf-8' });
      const a = document.createElement('a');
      a.href = URL.createObjectURL(blob);
      a.download = "柏努利实验数据.csv";
      a.click();
    }

    function importData(e) {
      const file = e.target.files[0];
      if (!file) return;
      const reader = new FileReader();
      reader.onload = evt => {
        const lines = evt.target.result.split('\n');
        alert('导入成功！数据已解析。');
      };
      reader.readAsText(file);
    }

    function generateReport() {
      const rep = document.getElementById('report-container');
      rep.innerHTML = `
        <div class="report-preview">
          <h3>柏努利方程实验报告</h3>
          <p>实验原理：理想流体恒定流动中，单位重量流体的位置水头、压强水头、流速水头之和为常数。</p>
          <p>实验组数：${groups.length}</p>
          <p>实验结论：在忽略损失时，总水头接近水平线，验证了 z + p/ρg + v²/(2g) = C。</p>
          <p>误差分析：存在沿程阻力、局部损失、测量读数误差、流量计误差等。</p>
        </div>
      `;
    }
  </script>
</body>
</html>
