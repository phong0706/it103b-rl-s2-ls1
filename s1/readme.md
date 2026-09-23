Nguyên nhân gây ra lỗi tính cước gấp rưỡi nằm ở nhánh else trong khối lệnh phân loại cước cơ sở. Ở biểu thức totalFare = baseFare + distanceInKm * extraFarePerKm;, hệ thống đang lấy toàn bộ tổng quãng đường nhân với cước phí phát sinh. Thực tế, 2 km đầu tiên đã được tính trọn gói trong cước cơ sở (baseFare), do đó, việc nhân tổng số km khiến 2 km đầu bị tính tiền lặp lại hai lần.

#
