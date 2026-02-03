# Crisis Response Flow – Building Management

```mermaid
flowchart TD

A[Nhận thông tin từ CQCN] --> B[Kích hoạt Tổ ứng phó nhanh]

B --> C{Phạm vi lây nhiễm?}

C -->|1 Tầng| D1[Cách ly 1 tầng]
C -->|1 Tầng làm khu CL| D2[Khu cách ly riêng]
C -->|1 Tòa| D3[Cách ly 1 tòa]
C -->|Toàn khu| D4[Cách ly toàn khu]

D1 --> E[Khoanh vùng vật lý]
D2 --> E
D3 --> E
D4 --> E

E --> F[Khóa toàn bộ luồng di chuyển]
F --> G[Thiết lập tiếp tế 1 chiều & thu rác]
G --> H[Duy trì vận hành tối thiểu]
H --> I[Truyền thông 1 đầu mối]
I --> J[Phối hợp CQCN liên tục]
