# soCoM
Repo này được kế thừa và sửa đổi từ code của paper gốc: 
'Semi-online Computational Offloading by Dueling Deep-Q Network for User Behavior Prediction'.
DOI: 10.1109/ACCESS.2020.3004861

Nó bao gồm

- soCoM.py: Mô hình hệ thống của model soCoM, bao gồm định nghĩa của các tác vụ, người dùng, server MEC, mô hình giao tiếp, mô hình tính toán và mô hình tiêu thụ năng lượng

- OFFLOAD.py: training mô hình RL cho quá trình giảm tải

- RLbrain*.py: Các thuật toán RL sử dụng

- Simulation.py: khởi tạo soCoM và môi trường mô phỏng
## Các thư viện
```
pip install -r requirement.txt
```
## Cách sử dụng
- Chạy file Simulation.py để sử dụng soCoM trong môi trường mô phỏng MEC

- Nếu muốn thay đổi số user equipment, thay đổi biến 'UN' trong file soCoM.py

- Nếu muốn sử dụng các thuật toán khác, thay đổi phần import các package trong file OFFLOAD.py và uncomment biến 'MODEL_USED' trong file soCoM.py