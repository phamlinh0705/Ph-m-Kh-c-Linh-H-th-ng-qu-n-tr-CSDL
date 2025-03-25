# Ph-m-Kh-c-Linh-H-th-ng-qu-n-tr-CSDL
Bài tập 2: K225480106037-Phạm Khắc Linh-Quản trị hệ quản trị cơ sở dữ liệu
BÀI TOÁN:
- Tạo csdl quan hệ với tên QLSV gồm các bảng sau:
  + SinhVien(#masv,hoten,NgaySinh)
  + Lop(#maLop,tenLop)
  + GVCN(#@maLop,#@magv,#HK)
  + LopSV(#@maLop,#@maSV,ChucVu)
  + GiaoVien(#magv,hoten,NgaySinh,@maBM)
  + BoMon(#MaBM,tenBM,@maKhoa)
  + Khoa(#maKhoa,tenKhoa)
  + MonHoc(#mamon,Tenmon,STC)
  + LopHP(#maLopHP,TenLopHP,HK,@maMon,@maGV)
  + DKMH(#@maLopHP,#@maSV,DiemTP,DiemThi,PhanTramThi)
  + Bài Làm :
 1. Tạo CSDL trên giao diện đồ họa
Tạo CSDL QLSV:
![image](https://github.com/user-attachments/assets/e1156f58-15a8-4508-bdd2-b097fd14c6b0)

Tạo các bảng dữ liệu
1. Tạo bảng sinh viên (#MaSV,Hoten,NgaySinh):
   ![image](https://github.com/user-attachments/assets/30bbf032-ddd4-4c91-8571-ea5439e4cbf1)
   ![image](https://github.com/user-attachments/assets/d82fc7a0-1019-4929-8c44-de9007106dc0)
   ![image](https://github.com/user-attachments/assets/c55d2210-fdf5-4165-93bf-416627af3a7a)

Tạo các bảng còn lại tương tự như các bước tạo bảng Sinhvien
 2. Tạo bảng lớp(#Malop,Tenlop):
![image](https://github.com/user-attachments/assets/c96ba430-2ee7-40fb-91b3-f2badedaf168)
3. Tạo bảng GVCN(#@Malop,#@MaGV,#HK):
![image](https://github.com/user-attachments/assets/3aa0ce03-dfb9-4785-9be9-4be551a8abb3)
4. Tạo bảng lớp sinh viên(#@Malop,#@MaSV,Chucvu):
![image](https://github.com/user-attachments/assets/29fa76ef-74de-47e2-87f5-6fcc7fc633ef)
5. Tạo bảng giáo viên (#MaGV,Hoten,Ngaysinh,@MaBM):
![image](https://github.com/user-attachments/assets/cbeb6d7b-19e1-46c7-9cf9-604a4caf2745)
6. Tạo bảng bộ môn (#MaBM,TenBM,@MaKhoa):
![image](https://github.com/user-attachments/assets/3307af8b-dfd1-44b6-86a0-48243a01c48f)
7. Tạo bảng Khoa (#Makhoa,Tenkhoa):
![image](https://github.com/user-attachments/assets/599a9d41-faaa-4782-a65a-2110f4093b29)
8. Tạo bảng môn học (#Mamon,Tenmon,STC):
![image](https://github.com/user-attachments/assets/47265fd6-5683-46e0-bf77-2068b2831f9a)
9. Tạo bảng lớp HP(#MaLopHP,TenLopHP,@Mamon,@MaGV):
![image](https://github.com/user-attachments/assets/d7613432-9908-4d7e-99d1-d1cec175810c)
10. Tạo bảng ĐKMH (#@MaLopHP, #@MaSV, DiemTP, DiemThi, PhanTramThi):
![image](https://github.com/user-attachments/assets/d458e2c4-f174-4cc7-ac26-c12ad9e54848)
Thiết lập các khóa FK, CK, PK cho bảng
1. Thiết lập khóa chính (PK) và khóa mở (CK) cho bảng SinhVien:
Thiết lập khóa khóa CK:
![image](https://github.com/user-attachments/assets/70b65def-5eb6-4edb-841c-e37708b6b08f)
![image](https://github.com/user-attachments/assets/889fa12a-b35d-4a2d-80b0-3ec95ecbfd59)
Sau khi nhập xong, nhấn tổ hợp phím Ctrl+S để lưu lại

2. Thiết lập khóa chính (PK) cho bảng Lop:
Làm tương tự các bước thiết lập khóa chính của bảng SinhVien:
![image](https://github.com/user-attachments/assets/624f8cf3-ed93-4ab6-8345-25e5f1c55efa)
3. Thiết lập khóa chính (PK) và khóa ngoại (FK) cho GVCN bảng:
Thiết lập khóa chính tương tự như các bảng trên
![image](https://github.com/user-attachments/assets/cb7495dc-02cf-4f2e-819a-68657e2e0028)
FK setting cho GVCN table:
![image](https://github.com/user-attachments/assets/0674915e-0455-42bc-aed0-5ae861f504ad)
![image](https://github.com/user-attachments/assets/26c81465-379d-46af-94d5-b272bc768e3a)
![image](https://github.com/user-attachments/assets/fc12e31e-767a-4574-9e9f-05ed82b1c924)
Sau khi nhập xong, nhấn tổ hợp phím Ctrl+S để lưu lại
Các bảng bên dưới tạo ra các khóa tương tự như các mô tả ở các bảng trên
4. Thiết lập khóa chính (PK) và khóa ngoại (FK) cho bảng LopSV
PK của bảng LopSV:
![image](https://github.com/user-attachments/assets/a02aa5d9-e7a5-4808-b5f8-18a3e6615813)
FK của bảng LopSV:
![image](https://github.com/user-attachments/assets/eac7d363-ae5d-454a-8ccb-b39769294c84)
5. PK, CK và FK của bảng GiaoViên
PK: (#MaGV)
![image](https://github.com/user-attachments/assets/b7cf0426-a8d6-4524-ae27-5ea5b55af517)
FK: (@MaBM)
![image](https://github.com/user-attachments/assets/357f5b87-05a7-4596-985c-99d16e97d677)
CK setting cho bảng GiaoViên:
![image](https://github.com/user-attachments/assets/0a6da768-5c9a-4d28-9b41-d6ec173203c1)
6. PK và FK của bảng BoMon
PK: (#MaBM):
![image](https://github.com/user-attachments/assets/a4aaa826-3d93-4993-bbba-717c81991d8b)
FK: (@MaKhoa):
![image](https://github.com/user-attachments/assets/9d8a0e0c-c9f9-4d2e-b259-7a70beb3c973)
7. PK của bảng Khoa
![image](https://github.com/user-attachments/assets/0f6911ac-588d-4fe7-a57f-6ec945127ea3)
8.PK của bảng MonHoc
![image](https://github.com/user-attachments/assets/fffa3fec-3c88-4012-abce-326ea95338ba)
9. PK và FK của bảng LopHP
PK: (#maLopHP):
![image](https://github.com/user-attachments/assets/49b11cbf-8999-48e7-be2e-f719f75e78ae)
FK: (@MaGV):
![image](https://github.com/user-attachments/assets/f5dc7373-05fd-4659-83ac-a0852337eca6)
FK: (@Mamon):
![image](https://github.com/user-attachments/assets/77ed5469-085e-4720-889a-85e4c46d64ec)
10. PK, FK, CK của bảng ĐKMH
PK của bảng DKMH:
![image](https://github.com/user-attachments/assets/71c5fa98-b3dd-489f-9dac-0fbbbf0c3a93)
FK: (@MaLopHP):
![image](https://github.com/user-attachments/assets/0fa94048-e9ca-4381-a93e-786d4a1bb73a)
FK: (@MaSV):
![image](https://github.com/user-attachments/assets/6a9514fc-b9f0-4d4b-9846-74160019a729)
CK setting cho ĐKMH bảng:
![image](https://github.com/user-attachments/assets/755e4d4c-7f9e-42d7-9655-d6ff1f302c04)
![image](https://github.com/user-attachments/assets/eeaa053c-28a2-4e9c-87bb-dd80bb3d312e)
![image](https://github.com/user-attachments/assets/fa343145-31fc-4c50-8ef6-067f49679caa)
2. Chuyển các thao tác đồ họa thành lệnh SQL tương thích
   ![image](https://github.com/user-attachments/assets/daa79f14-0855-4175-be98-8622bb7fe714)
   Lệnh SQL sau khi chuyển từ thao tác đồ họa của bảng SinhVien
![image](https://github.com/user-attachments/assets/6d008295-eab5-4872-bfc9-bcbef76f3f3b)
- Các SLQ lệnh chuyển sang bảng tương tự khác như cách thực hiện


