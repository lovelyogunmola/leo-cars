# EASIEST WAY: use admin.html
Open https://lovelyogunmola.github.io/leo-cars/admin.html on your phone, log in with your GitHub token, then change a car to Sold or post a new car with photos and videos.

---
# Manual way (without admin page)

Open your repo `leo-cars` in the GitHub app or github.com. All cars live in `cars.json`.

## Mark a car SOLD (or RESERVED)
1. Open `cars.json`, tap the pencil (Edit).
2. Find the car, change `"status": "available"` to `"status": "sold"` (or `"reserved"`).
3. Commit changes. The site updates in about a minute.
Sold cars turn grey, show a SOLD badge, move to the bottom, and the button becomes "Ask for similar".

## Add a new car
1. Upload the photos to the `images` folder (Add file > Upload files) and videos to `videos`.
   For each video also upload a cover picture with the same name (car.mp4 + car.jpg).
2. In `cars.json`, copy one car block, paste it after the last `}` with a comma, and change:
   year, name, country, details (put mileage here), price (0 = "Price on WhatsApp"),
   note (e.g. "Shipping to Lagos included"), photos, videos.
3. Commit changes.

Tips: keep each video under about 1 MB (short and compressed) and photos under 200 KB.
Blur license plates before uploading. Watch the commas in cars.json: one missing comma breaks the list.
