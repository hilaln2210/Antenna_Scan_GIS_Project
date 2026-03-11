# Antenna Scan GIS Project

מיפוי אנטנות סלולריות בישראל — פרויקט GIS לאיתור ומיקום אנטנות.
ריכוז מידע ממקורות שונים (מינהל הקרינה הסביבתית) בממשק ידידותי ואינטראקטיבי.

---

## צילומי מסך

### דף בית
![דף בית](screenshots/home.png)

### מפת אנטנות (8,076 אנטנות + clustering + פילטרים)
![מפת אנטנות](screenshots/map.png)

### דירוג ומשוב
![דירוג](screenshots/rating.png)

### התחברות
![התחברות](screenshots/login.png)

### הרשמה
![הרשמה](screenshots/register.png)

### הרשמה הצליחה
![הצלחה](screenshots/success.png)

---

## תכונות

- **דף בית** — כניסה לאפליקציה
- **Login / Register** — התחברות והרשמה (כולל דף אישור)
- **Map** — מפת אנטנות אינטראקטיבית עם:
  - **Marker Clustering** — אגירת 8,076 נקודות לביצועים מיטביים
  - **סרגל סטטיסטיקות** — לפי חברה, רמת קרינה, ו-10 ערים מובילות
  - **פילטרים** — לפי חברה, רמת קרינה, עיר (עם autocomplete)
  - **Popup מפורט** — כולל טכנולוגיה, תאריכי היתר, קישורים למסמכים
  - **שכבות מפה** — Street Map / Satellite
- **Rating and Opinion** — דירוג ומשוב עם:
  - דירוג כוכבים אינטראקטיבי (1–5)
  - שמירת ביקורות ב-localStorage
  - תצוגת ביקורות קהילתיות

---

## טכנולוגיות

- **HTML · CSS · JavaScript**
- **Leaflet.js** — מפות אינטראקטיביות
- **Leaflet.markercluster** — clustering ביצועי
- **Leaflet-Control-Geocoder** — חיפוש מיקום
- **OpenStreetMap / Esri Satellite** — שכבות מפה

---

## הרצה

```bash
# שרת מקומי
python3 -m http.server 8000
# פתחי בדפדפן: http://localhost:8000/Home.html
```

---

## קבצים עיקריים

| קובץ | תיאור |
|------|-------|
| `Home.html` | דף בית |
| `login.html` | התחברות |
| `Register.html` | הרשמה |
| `registration_success.html` | אישור הרשמה |
| `map.html` | מפת אנטנות |
| `rating_opinion.html` | דירוג ומשוב |
| `DATA_converted.json` | נתוני אנטנות (8,076 רשומות) |

---

## נתונים

הנתונים מקורם ממינהל הקרינה הסביבתית — משרד הסביבה ישראל.
כל אנטנה כוללת: מיקום GPS, חברה, סוג אתר, עוצמת קרינה, תאריכי היתר, ומסמכים רשמיים.

---

## מסמך פרויקט

- `cellular antennas mapping - GIS project - Hila Mendelson.pdf`

---

© Hila · GIS Project
