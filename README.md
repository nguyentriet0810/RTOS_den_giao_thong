# RTOS_den_giao_thong

1. Đề: Viết OS quản lý tín hiệu đèn giao thông với yêu cầu:
    Auto: đèn xanh 26s đèn vàng 4s đèn đỏ 30s
    Manual: nhấp nháy đèn vàng chu kì 2s
    Chuyển task bằng cách nhấn nút

2. Kết nối phần cứng:
    MCU stm32 blue pill (stm32f103c8t6)
    Pa0 cấu hình ngắt ngoài nhận tín hiệu từ nút nhấn (limit switch)
    Pa1 đèn đỏ 1
    Pa2 đèn vàng 1
    Pa3 đèn xanh 1
    Pa4 đèn đỏ 2
    Pa5 đèn vàng 2
    Pa6 đèn xanh 2

3. Các file trong project:
    main.c: chứa chương trình thực thi của các task và các hàm xử lý ngắt
    main.h: chứa các thư viện dùng trong project và các nguyên mẫu hàm
    OSkernel.c: chứa các chương trình thực thi của 1 os cơ bản
    OSkernel.h: chứa các thư viện cần dùng và nguyên mẫu hàm
    OSkernel.s (assembly): chứa chương trình khởi chạy task đầu tiên của hệ thống và chương trình sao lưu, khôi phục, chuyển các task




