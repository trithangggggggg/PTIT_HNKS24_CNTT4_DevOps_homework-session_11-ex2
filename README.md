# Bài 2: Biên dịch đóng gói tệp ứng dụng .jar với Gradle và lưu trữ Artifacts

## Mục tiêu
- Thực thi câu lệnh biên dịch và đóng gói ứng dụng Spring Boot thành tệp thực thi `.jar` bằng Gradle (`./gradlew bootJar`).
- Lưu trữ thành phẩm biên dịch (`.jar`) từ thư mục `build/libs/` lên GitHub Actions bằng `actions/upload-artifact@v4`.

## Các bước cấu hình bổ sung
1. **Đóng gói tệp JAR**: `run: ./gradlew bootJar`
2. **Lưu trữ Artifacts**:
   - Action: `actions/upload-artifact@v4`
   - Artifact name: `app-jar`
   - File path: `build/libs/*.jar`
