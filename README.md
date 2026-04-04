# SD-WAN

Sơ đồ đầu tiên của nhóm phát triển

<img width="505" height="593" alt="image" src="https://github.com/user-attachments/assets/344baeeb-1dcf-40d3-8bf0-5dabda45d2f6" />

Thành quả: Loadbalancing ổn định qua 2 đường WAN1(từ pfsense đến R1) và WAN2(từ pfsense đến R2).

Ý tưởng cải tiến: Từ SD-WAN cơ bản thành High Availability SD-WAN Architecture thêm 1 con pfsense nữa để đề phòng trường hợp chẳng may bị hư thì không ảnh hưởng tới đường mạng, chỉ cần hệ thống mạng không bị hư quá 2/3 thì vẫn có thể hoạt động được.

<img width="683" height="640" alt="image" src="https://github.com/user-attachments/assets/3adecda5-a675-44ef-abb1-1ff5e540efda" />

Thách thức: Cấu hình sẽ vất vả hơn vì phải đảm bảo định tuyến đúng tránh trường hợp Routing Loop, giải quyết vấn đề đồng bộ hóa trạng thái(High Availability - HA)

