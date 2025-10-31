# JB-IOC-PTHB251027_HuynhAnhQuoc_MD1_Session1_XS_QLBanVeSuKien
JVBE - MD1: BTVN QLSKBVTT (XS)

Logic nghiệp vụ ngăn chặn quá số lượng vé còn lại sẽ là:

Khi một người dùng tạo Booking (hoặc chuyển Booking sang trạng thái "paid"), hệ thống phải kiểm tra: SUM(BookingDetail.SL) của tất cả các Booking (ở trạng thái pending hoặc paid) cho một ticket_type_id cụ thể PHẢI <= TicketType.SL tối đa. Nếu vượt quá, giao dịch sẽ thất bại.
