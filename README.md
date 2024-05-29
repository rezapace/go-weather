# Cuaca Golang 🌦️

Selamat datang di proyek Cuaca Golang! Proyek ini dibuat untuk memberikan informasi cuaca yang akurat dan terkini menggunakan bahasa pemrograman Golang. Dengan menggunakan API cuaca, proyek ini menyajikan data cuaca yang mudah dibaca dan diintegrasikan ke dalam proyek Golang Anda.

## Cara Menjalankan

1. **Clone repository:**
    ```bash
    git clone https://github.com/rezapace/cuaca_go
    ```

2. Install dependencies:
    ```bash
    go mod tidy
    ```

3. Jalankan aplikasi:
    ```bash
    go run main.go
    ```

4. Gunakan Postman untuk mengakses API:
    ```bash
    http://localhost:8080/weather?location=jakarta
    ```

## Dokumentasi API

### Endpoint: Get Weather

- **URL:** `/weather`
- **Method:** `GET`
- **Query Parameters:**
  - `location` (string): Nama lokasi untuk mendapatkan informasi cuaca.

- **Contoh Request:**
    ```http
    GET http://localhost:8080/weather?location=jakarta
    ```

- **Deskripsi:** Mendapatkan cuaca dari API eksternal dan menjalankan menggunakan framework Echo.

## Contoh Response

```json
{
  "location": {
    "name": "Jakarta",
    "region": "Jakarta Raya",
    "country": "Indonesia",
    "lat": -6.2,
    "lon": 106.8,
    "tz_id": "Asia/Jakarta",
    "localtime_epoch": 1618317040,
    "localtime": "2021-04-13 10:30"
  },
  "current": {
    "temp_c": 30.0,
    "condition": {
      "text": "Partly cloudy",
      "icon": "//cdn.weatherapi.com/weather/64x64/day/116.png",
      "code": 1003
    },
    "wind_kph": 15.0,
    "humidity": 70,
    "cloud": 50,
    "feelslike_c": 32.0
  }
}
```

## Gambar

![Running Echo](https://github.com/rezapace/cuaca_go/blob/main/output/runing%20echo.jpg?raw=true)
![Postman Output](https://github.com/rezapace/cuaca_go/blob/main/output/postman%20output.jpg?raw=true)

Terima kasih telah menggunakan Cuaca Golang! 🌤️💻

