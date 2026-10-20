# Tổ chức thư mục bằng GUI

**A2. Đổi tên thư mục gốc thành trung-tam-tieng-anh.**

```
1 Rename-Item "Trung Tam Tieng Anh FINAL" trung-tam-tieng-anh
2 cd trung-tam-tieng-anh
```

**A3. Tạo 5 thư mục trong thư mục gốc: docs, media, data, logs, archive.**

```
1 mkdir docs, media, data, logs, archive
```

**A4. Đổi tên đúng 5 file Logo Trung Tam.PNG, Anh Lop Hoc.JPG, Lich Hoc.txt, Hoc Vien Khoa 3.xlsx, Access.log theo dạng snake_case.**

```
1 Rename-Item "Logo Trung Tam.PNG" logo_trung_tam.png

2 Rename-Item "Anh Lop Hoc.JPG" anh_lop_hoc.jpg

3 Rename-Item "Lich Hoc.txt" lich_hoc.txt

4 Rename-Item "Hoc Vien Khoa 3.xlsx" hoc_vien_khoa_3.xlsx

5 Rename-Item "Access.log" access.log

6 **A
```

**5. Dùng GUI chuyển file Excel vào data, file log vào logs. Giữ logo, ảnh lớp học, file lịch học và 2 file .tmp tại thư mục gốc để làm Phần B.**

```
1 Move-Item hoc_vien_khoa_3.xlsx data
2 Move-Item access.log logs
```

**A6. Sao chép mẫu** [**bai_lam_ngay1.md**](http://bai_lam_ngay1.md) **vào thư mục gốc. Giữ .env ở thư mục gốc** Copy-Item ../[bai_lam_ngay1.md](http://bai_lam_ngay1.md) ./

```
1 Copy-Item ../bai_lam_ngay1.md ./
2 Copy-Item ../bai_lam_ngay1.md ./

logo_trung_tam.png, anh_lop_hoc.jpg, lich_hoc.txt, temp_201.tmp, temp_202.tmp, .env, bai_lam_ngay1.md

dir -Force
```
# Thao tác bằng GLI
## Phần B
-   B1: pwd
Kết quả B1 : C:\Users\TenBan\Desktop\starter-kit\trung-tam-tieng-anh
-   B2 : dir -Force
-   B3 : Move-Item lich_hoc.txt docs/
           Move-Item logo_trung_tam.png media/
           Move-Item anh_lop_hoc.jpg media/
-   B4 : Copy-Item media/logo_trung_tam.png archive/
-   B5 : Remove-Item temp_202.tmp
-   B6 : cd ./logs ; dir -Force ; cd ..
-   B7 : cd docs ; Copy-Item            ../media/anh_lop_hoc.jpg ../archive/ ; cd ..
-   B8 :Get-ChildItem -Recurse -Force
