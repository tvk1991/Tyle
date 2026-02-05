---
layout: default
title: Bảng Tính Hoa Hồng CTV
---

<div class="container">
    <header>
        <h1><i class="fas fa-calculator"></i> Bảng Tính Hoa Hồng CTV</h1>
        <p class="subtitle">Tính hoa hồng theo tỷ lệ 0.4% cho BILL A và 0.2% cho BILL B</p>
    </header>
    
    <div class="instructions" id="huong-dan">
        <h3><i class="fas fa-info-circle"></i> Hướng dẫn sử dụng</h3>
        <div class="instructions-content">
            <div class="instructions-section">
                <h4><i class="fas fa-keyboard"></i> Cách nhập liệu</h4>
                <ul>
                    <li>Nhấn vào ô BILL A hoặc BILL B để chọn ô cần nhập</li>
                    <li>Sử dụng bàn phím ảo 3x3 để nhập số tiền</li>
                    <li>Nhấn "Tiếp" để chuyển sang ô tiếp theo</li>
                    <li>Nhấn "OK" để xác nhận và đóng bàn phím</li>
                </ul>
            </div>
            <div class="instructions-section">
                <h4><i class="fas fa-calculator"></i> Công thức tính</h4>
                <ul>
                    <li><strong>Hoa hồng A:</strong> BILL A × 0.4%</li>
                    <li><strong>Hoa hồng B:</strong> BILL B × 0.2%</li>
                    <li><strong>Tổng hàng:</strong> Hoa hồng A + Hoa hồng B</li>
                    <li>Kết quả tự động tính và làm tròn số</li>
                </ul>
            </div>
        </div>
    </div>
    
    <div class="calculator-container" id="tinh-toan">
        <div class="formula-display">
            <div class="formula-text">
                <strong>Công thức:</strong> 
                <span>BILL A × 0.4%</span> + 
                <span>BILL B × 0.2%</span> = 
                <span>Tổng hoa hồng</span>
            </div>
            <div class="current-time" id="currentTime">Đang cập nhật thời gian...</div>
        </div>
        
        <!-- Wrapper cho bảng để cuộn ngang trên mobile -->
        <div class="table-responsive">
            <table id="calculationTable">
                <thead>
                    <tr>
                        <th width="8%">STT</th>
                        <th width="22%">BILL (A) vnđ</th>
                        <th width="18%">0.4% vnđ</th>
                        <th width="22%">BILL (B) vnđ</th>
                        <th width="18%">0.2% vnđ</th>
                        <th width="12%">Tổng vnđ</th>
                    </tr>
                </thead>
                <tbody id="tableBody">
                    <!-- Hàng dữ liệu sẽ được thêm tự động -->
                </tbody>
                <tfoot>
                    <tr class="total-row">
                        <td><strong>TỔNG</strong></td>
                        <td id="totalAInput" class="result-cell">0 vnđ</td>
                        <td id="totalA" class="result-cell">0 vnđ</td>
                        <td id="totalBInput" class="result-cell">0 vnđ</td>
                        <td id="totalB" class="result-cell">0 vnđ</td>
                        <td id="grandTotal" class="result-cell grand-total-cell">0 vnđ</td>
                    </tr>
                </tfoot>
            </table>
        </div>
        
        <div class="action-buttons" id="xuat-excel">
            <button id="addRowBtn">
                <i class="fas fa-plus-circle"></i> Thêm Hàng Mới
            </button>
            <button id="deleteRowBtn">
                <i class="fas fa-trash-alt"></i> Xóa Hàng Cuối
            </button>
            <button id="resetBtn">
                <i class="fas fa-redo-alt"></i> Đặt Lại Bảng Tính
            </button>
            <button id="exportExcelBtn">
                <i class="fas fa-file-excel"></i> Xuất ra Excel
            </button>
        </div>
    </div>
    
    <div class="footer" id="lien-he">
        <div class="export-info">
            <p><i class="fas fa-download"></i> File Excel xuất ra sẽ có định dạng tiền Việt Nam: 1.000 TR</p>
            <p><i class="fas fa-calendar-alt"></i> Tên file tự động chứa ngày giờ xuất báo cáo</p>
            <p><i class="fas fa-keyboard"></i> Sử dụng bàn phím ảo 3x3 để nhập liệu dễ dàng</p>
        </div>
        <div>
            <p>Bảng tính / Hoa Hồng CTV ©2026</p>
            <p id="lastExportInfo">Chưa có file nào được xuất</p>
            <p>Thiết Kế Bởi 21 Quân sự</p>
            <p>https://tvk1991.github.io/hoahong/</p>
        </div>
    </div>
</div>
