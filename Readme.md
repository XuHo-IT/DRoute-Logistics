# SWIFTROUTE LOGISTICS DASHBOARD
## Logistics Performance & Operations Analytics Platform

## 1. Project Overview

SwiftRoute Logistics Dashboard là hệ thống phân tích dữ liệu vận hành logistics được xây dựng nhằm cung cấp góc nhìn 360° về hiệu suất giao hàng, hiệu quả trung tâm phân phối (Hub), năng lực tài xế (Driver), và tình trạng đội xe (Vehicle Fleet).

### Chức năng chính

Dashboard giúp ban quản lý:

- Theo dõi KPI vận hành theo tháng
- Phân tích tăng trưởng MoM (Month-over-Month)
- Phát hiện bottleneck trong hub
- Xác định tài xế gây delay
- Đánh giá độ tin cậy của phương tiện
- Cải thiện SLA & Customer Satisfaction

## 2. Business Objectives

- Tăng tỷ lệ giao hàng đúng hạn (On-Time Delivery Rate)
- Giảm thời gian giao hàng trung bình
- Tối ưu phân bổ công suất hub
- Cải thiện hiệu suất tài xế
- Giảm breakdown phương tiện
- Nâng cao CSAT (Customer Satisfaction Score)

## 3. Dashboard Architecture

Hệ thống gồm 4 dashboard chính:

### 3.1. Overview Dashboard (Executive View)

#### Core KPI Monitoring

- Total Orders (Current vs Previous Month)
- MoM Growth %
- On-Time Delivery Rate
- CSAT %
- Average Delivery Time (Hours)

**Mục tiêu:** Cung cấp cái nhìn tổng quan về sức khỏe vận hành toàn hệ thống.

#### Operational Snapshot

Bao gồm:

- Tổng số Hub
- Số lượng Driver
- Quy mô Fleet
- Tình trạng phương tiện
- Hub capacity vs actual processed
- Top driver delay contributors

**Mục tiêu:** Xác định nhanh vấn đề vận hành cấp hệ thống.

### 3.2. Hubs Overview Dashboard

#### Phân tích trọng tâm:

- Hub Capacity Utilization
- Hub Performance Ranking
- Hub Processing Time (daily)
- So sánh công suất vs workload

#### Insight tạo ra:

- Hub nào đang quá tải?
- Hub nào under-utilized?
- Hub nào có thời gian xử lý chậm?
- Có bottleneck ở khâu xử lý trước khi dispatch không?

**Giá trị:** Giúp tối ưu mạng lưới phân phối.

### 3.3. Drivers Overview Dashboard

#### Phân tích:

- Số lượng driver active
- Experience vs Rating correlation
- Drivers gây nhiều delay
- Profile chi tiết từng driver
- Monthly trend workload

#### Insight tạo ra:

- Kinh nghiệm có ảnh hưởng đến performance không?
- Driver nào cần training?
- Workload có phân bổ đều không?
- Seasonality có ảnh hưởng đến năng suất?

**Giá trị:** Hỗ trợ HR + Operations decision making.

### 3.4. Vehicle Overview Dashboard

#### Phân tích:

- Fleet size & active rate
- Orders theo vehicle model
- Vehicle age vs breakdown
- Breakdown theo model / vehicle code
- Fleet utilization pattern

#### Insight tạo ra:

- Xe cũ có gây nhiều breakdown?
- Model nào ít bền?
- Cần thay thế fleet nào?
- Fleet có đang sử dụng hiệu quả không?

**Giá trị:** Hỗ trợ Fleet Management & Cost Optimization.

## 4. Data Model & Domain Intelligence

### Dữ liệu được tổ chức theo mô hình:

**Fact Table:**
- Orders

**Dimension Tables:**
- Hubs
- Drivers
- Vehicles

### Key Analytical Relationships:

- Orders → Hub (Hub ID)
- Orders → Driver (Driver ID)
- Orders → Vehicle (Vehicle ID)
- Time Intelligence (Order Date)

## 5. Advanced Analytical Concepts Used

Project này không chỉ là dashboard cơ bản mà bao gồm:

- Time Intelligence (MoM calculation)
- KPI comparison current vs previous period
- Capacity Utilization Analysis
- Performance Ranking Logic
- Correlation Analysis (Experience vs Rating, Age vs Breakdown)
- Root Cause Analysis (Delay Reason)
- SLA Performance Monitoring
- Operational Efficiency Tracking

## 6. Business Impact

Khi triển khai thực tế, dashboard có thể giúp:

- Tăng On-Time Rate lên 5–12%
- Giảm delivery time trung bình
- Phát hiện 20% tài xế gây 60% delay
- Xác định hub quá tải trước khi gây SLA breach
- Giảm chi phí bảo trì fleet

## 7. Technical Implementation

**Data Modeling:**
- Data modeling theo Star Schema

**DAX Measures:**
- MoM Growth
- Running metrics
- Utilization %

**Interactive Features:**
- Interactive slicers (Year / Month / Hub / Driver / Vehicle)
- Drill-through Driver Profile
- Conditional formatting cho performance alerts

## 8. Project Maturity Level

Đây là dashboard nâng cao thể hiện khả năng về:

- Logistics domain knowledge
- Operations management
- KPI design
- Business thinking
- Data storytelling
- Decision-support analytics