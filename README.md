# DATA-WAREHOUSE
BULD DATA WAREHOUSE ANALYSIS OF SUPPLY CHAINS DATA (PHÂN TÍCH DỮ LIỆU CHUỖI CUNG ỨNG)
## 1. Giới thiệu:
Bộ dữ liệu DataCo Smart Supply Chain for Big Data Analysis trên Kaggle là một tập hợp các dữ liệu về chuỗi cung ứng thông minh, bao gồm thông tin về đơn hàng, sản phẩm, khách hàng và các hoạt động vận chuyển liên quan. Bộ dữ liệu này cung cấp cho chúng ta một cái nhìn tổng quát về hoạt động của các doanh nghiệp trong lĩnh vực này và có thể được sử dụng để phân tích và tối ưu hóa các quy trình kinh doanh liên quan đến chuỗi cung ứng. Tôi có thể sử dụng bộ dữ liệu này để tìm hiểu về xu hướng và mối quan hệ giữa các yếu tố khác nhau trong chuỗi cung ứng, từ đó đưa ra các khuyến nghị và giải pháp để cải thiện hiệu quả và giảm chi phí cho các hoạt động kinh doanh.
Link Dataset: https://www.kaggle.com/datasets/shashwatwork/dataco-smart-supply-chain-for-big-data-analysis?select=DataCoSupplyChainDataset.csv
## 2. Lược đồ hình sao:
![Screenshot 2023-05-21 175015](https://github.com/thanhtin99/DATA-WAREHOUSE/assets/95009162/20f6d88d-8974-4e89-942d-b4c26139c085)
## 3. Nội dung chính:
### 3.1 Xây dựng kho dữ liệu bằng công cụ SSIS
- Tạo CoSupply_Stage lưu trữ các table stage và CoSupply_DW  lưu trữ các tabel Dim - Fact
- Đổ dữ liệu từ excel vào các bảng stage
  ![image](https://github.com/thanhtin99/DATA-WAREHOUSE/assets/95009162/bebb4a2e-a621-4a4c-a712-3a6b54c51daa)

- Đổ dữ liệu từ stage vào các bảng Dim và Fact
  ![image](https://github.com/thanhtin99/DATA-WAREHOUSE/assets/95009162/adf5b628-eae7-4d0d-91d1-84418d6b635f)

- Tạo các khoá ngoại giữa các bảng Fact và các bảng Dim
### 3.2 Xây dựng cube và truy vấn bằng công cụ SSAS
- Tạo Data Source từ kho dữ liệu database CoSupply_DW
- Tạo Data Source View
- Tạo cube, thêm measure và các dim cần thiết,tạo các phân cấp
- Truy vấn các câu hỏi bằng công cụ SSAS, Pivot Table, PowerBI
![image](https://github.com/thanhtin99/DATA-WAREHOUSE/assets/95009162/3a9f82c1-119c-4644-b1e1-d4a002e5474e)
Truy vấn dữ liệu sử dụng SSAS
![image](https://github.com/thanhtin99/DATA-WAREHOUSE/assets/95009162/01754ffd-cfeb-4770-8f7e-2a7027c6860e)
![image](https://github.com/thanhtin99/DATA-WAREHOUSE/assets/95009162/58ac9b4b-84bd-4ede-a449-b1c231209286)
Truy vấn dữ liệu sử dụng Pivot Table
![image](https://github.com/thanhtin99/DATA-WAREHOUSE/assets/95009162/11aadc46-dda9-433d-9b02-5c64ada51038)
Truy vấn sử dụng Power BI
![image](https://github.com/thanhtin99/DATA-WAREHOUSE/assets/95009162/5b4ac017-57d3-4513-b6ec-cb1b83158647)
![image](https://github.com/thanhtin99/DATA-WAREHOUSE/assets/95009162/299cc24f-de26-4c01-9f2e-08729247551a)
![image](https://github.com/thanhtin99/DATA-WAREHOUSE/assets/95009162/0d787a1d-aeab-4e9b-830f-3c1b29c95e89)
![image](https://github.com/thanhtin99/DATA-WAREHOUSE/assets/95009162/59b44bf4-73ec-40cb-b396-2389d45ef8da)




