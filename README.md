[code htm.txt](https://github.com/user-attachments/files/22062252/code.htm.txt)
<!doctype html>
<html lang="vi">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Bảng lương tối thiểu vùng mới nhất</title>
  <meta name="description" content="Bảng tra cứu mức lương tối thiểu vùng (áp dụng từ Nghị định), thiết kế đơn giản, tinh tế, có hình ảnh minh họa." />
  <style>
    :root{--bg:#fbfbfb;--card:#ffffff;--muted:#6b6b6b;--accent:#0b6efd;--glass:rgba(11,110,253,0.06)}
    *{box-sizing:border-box}
    body{font-family:Inter, ui-sans-serif, system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial; margin:0; background:linear-gradient(180deg,var(--bg),#f3f6ff); color:#0f172a}
    .wrap{max-width:920px;margin:36px auto;padding:24px}
    header{display:flex;align-items:center;gap:16px;margin-bottom:18px}
    .brand{display:flex;gap:12px;align-items:center}
    .logo{width:56px;height:56px;border-radius:12px;display:grid;place-items:center;background:var(--glass);box-shadow:0 6px 18px rgba(12,40,80,0.06)}
    h1{font-size:20px;margin:0}
    p.lead{margin:6px 0 18px;color:var(--muted);font-size:14px}
    .hero{display:grid;grid-template-columns:1fr 220px;gap:18px;align-items:center;margin-bottom:22px}
    .card{background:var(--card);border-radius:12px;padding:18px;box-shadow:0 6px 18px rgba(12,40,80,0.04)}
    .illustration{width:100%;height:140px;display:flex;align-items:center;justify-content:center}
    table{width:100%;border-collapse:collapse;margin-top:8px}
    th,td{padding:10px 12px;border-bottom:1px solid #eef2ff;text-align:left}
    th{background:linear-gradient(90deg,#f8fbff,#ffffff);font-weight:600}
    .note{font-size:13px;color:var(--muted);margin-top:12px}
    .meta{font-size:13px;color:var(--muted);display:flex;gap:8px;align-items:center}
    .cta{margin-top:14px;display:flex;gap:8px;flex-wrap:wrap}
    .btn{padding:8px 12px;border-radius:8px;border:1px solid rgba(11,110,253,0.12);background:linear-gradient(180deg,#fff,#f3f8ff);cursor:pointer}
    footer{margin-top:28px;font-size:13px;color:var(--muted);text-align:center}
    @media (max-width:720px){.hero{grid-template-columns:1fr;}.illustration{height:120px}}
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <div class="brand">
        <div class="logo" aria-hidden="true">
          <!-- simple lotus svg -->
          <svg width="34" height="34" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
            <path d="M12 3s3 3 5 6c2 3-1 6-5 9-4-3-7-6-5-9 2-3 5-6 5-6z" fill="#0b6efd" opacity="0.12"/>
            <path d="M12 3s3 3 5 6c2 3-1 6-5 9-4-3-7-6-5-9 2-3 5-6 5-6z" stroke="#0b6efd" stroke-width="1.25" fill="none" stroke-linecap="round" stroke-linejoin="round"/>
          </svg>
        </div>
        <div>
          <h1>Bảng lương tối thiểu vùng mới nhất</h1>
          <div class="meta">Áp dụng theo nghị định | <time datetime="2025-07-01">Cập nhật: 01 Jul 2025</time></div>
        </div>
      </div>
    </header>

    <div class="hero">
      <div class="card">
        <p class="lead">Bảng tra cứu nhanh mức lương tối thiểu theo 4 vùng. Dùng để tham khảo khi tính lương, đóng BHXH hoặc soạn thảo chế độ trả lương. Luôn kiểm tra văn bản pháp luật chính thức để đảm bảo tuân thủ.</p>

        <!-- Data table -->
        <h3 style="margin-top:6px;margin-bottom:6px">Mức lương tối thiểu vùng (VND / tháng)</h3>
        <div style="overflow:auto">
          <table role="table" aria-label="Bảng lương tối thiểu vùng">
            <thead>
              <tr><th scope="col">Vùng</th><th scope="col">Mức lương (đồng/tháng)</th><th scope="col">Mức giờ (đồng/giờ)</th><th scope="col">Ghi chú</th></tr>
            </thead>
            <tbody>
              <tr><td>Vùng I</td><td>4.960.000</td><td>23.800</td><td>Áp dụng cho các đô thị, tỉnh trung tâm</td></tr>
              <tr><td>Vùng II</td><td>4.410.000</td><td>21.200</td><td>Khu vực có mức sống trung bình</td></tr>
              <tr><td>Vùng III</td><td>3.860.000</td><td>18.600</td><td>Vùng nông thôn, ít phát triển</td></tr>
              <tr><td>Vùng IV</td><td>3.450.000</td><td>16.600</td><td>Mức thấp nhất theo quy định hiện hành</td></tr>
            </tbody>
          </table>
        </div>

        <p class="note">Nguồn: Nghị định liên quan về lương tối thiểu vùng (áp dụng từ 01/7/2024) và các cập nhật chính thức của Chính phủ. Đây là dữ liệu tham khảo; vui lòng kiểm tra trang chính phủ hoặc văn bản pháp luật để xác thực.</p>

        <div class="cta">
          <button class="btn" onclick="copyCSV()">Sao chép CSV</button>
          <button class="btn" onclick="printTable()">In bảng</button>
        </div>

      </div>

      <aside class="card" style="display:flex;flex-direction:column;gap:12px;align-items:center">
        <div class="illustration">
          <!-- stylized map pin / chart -->
          <svg width="160" height="120" viewBox="0 0 160 120" fill="none" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
            <rect x="0" y="0" width="160" height="120" rx="12" fill="#f7fbff"/>
            <path d="M40 80 L60 50 L80 68 L100 40 L120 56" stroke="#0b6efd" stroke-width="3" fill="none" stroke-linecap="round" stroke-linejoin="round" opacity="0.95"/>
            <circle cx="40" cy="80" r="4" fill="#0b6efd"/>
            <circle cx="120" cy="56" r="4" fill="#0b6efd"/>
          </svg>
        </div>
        <div style="text-align:center">
          <strong>Áp dụng</strong>
          <div class="meta">Từ 01 Jul 2024 • Cập nhật 2025</div>
        </div>
      </aside>
    </div>

    <section style="margin-top:6px">
      <div class="card">
        <h3>Giải thích nhanh</h3>
        <ul style="margin-top:6px">
          <li>Lương tối thiểu vùng là mức lương thấp nhất mà người lao động làm công ăn lương được hưởng theo quy định pháp luật.</li>
          <li>Đơn vị tính: đồng/tháng (áp dụng cho hợp đồng lao động theo tháng). Mức giờ được quy đổi tương đương theo thời giờ làm việc tiêu chuẩn.</li>
          <li>Những trợ cấp, phụ cấp, tiền thưởng khác có thể vẫn được trả theo thỏa thuận, doanh nghiệp không được dùng mức lương tối thiểu để cắt các quyền lợi hiện hành.</li>
        </ul>
        <p class="note">⚠️ Lưu ý: thông tin trên trang mang tính tham khảo. Để hoàn toàn chính xác, xem Nghị định của Chính phủ hoặc trang Thư viện Pháp luật.</p>
      </div>
    </section>

    <footer>
      © <span id="year"></span> Bảng lương tối thiểu vùng — Thiết kế đơn giản, tinh tế
    </footer>
  </div>

  <script>
    document.getElementById('year').textContent = new Date().getFullYear();
    function copyCSV(){
      const rows = [['Vùng','Lương (đồng/tháng)','Lương (đồng/giờ)'],['Vùng I','4960000','23800'],['Vùng II','4410000','21200'],['Vùng III','3860000','18600'],['Vùng IV','3450000','16600']];
      const csv = rows.map(r=>r.map(c=>'"'+c+'"').join(',')).join('\n');
      navigator.clipboard.writeText(csv).then(()=>alert('Đã sao chép CSV vào clipboard'))
    }
    function printTable(){ window.print(); }
  </script>
</body>
</html>
