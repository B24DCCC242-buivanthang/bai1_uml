@startuml
class Vehicle {
  - biển số: string
  - hãng xe: string
  - màu xe: string
  - số chỗ ngồi: int
  - năm sản xuất: number
  - tài xế: string

  + khởi động()
  + tắt máy()
  + tăng tốc()
  + phanh()
}

class "Xe ô tô" as Car {
  - điểm đón: string

  + đón khách()
  + trả khách()
}

class "Xe buýt" as Bus {
  - tuyến xe: string

  + tuyến đường cố định()
  + nhiều chuyến()
  + đón khách()
  + trả khách()
  + hoạt động theo giờ()
}

Vehicle <|-- Car
Vehicle <|-- Bus
@enduml
