# Samia’s Closet — Guest Order Version

এই version-এ:
- Customer signup/login নেই
- Customer account/order history নেই
- Quiz, voucher, mystery box, streak, reward system নেই
- শুধু owner Admin Login আছে
- Guest customer signup ছাড়াই order করতে পারে
- bKash + Nagad: 01314652599
- Cash on Delivery রাখা আছে
- Moulvibazar delivery ৳50
- Moulvibazar-এর বাইরে delivery ৳150
- Online payment-এ Transaction ID + optional payment screenshot
- Admin order status ও queue position control করতে পারে
- Product add/delete করতে পারে

## Firebase
`app.js`-এ `REPLACE_WITH_YOUR_FIREBASE_API_KEY`-এর জায়গায় তোমার Firebase Web API key বসাও।

Firebase Authentication-এ শুধু admin email/password account রাখবে:
rahihumaun369@gmail.com

Firestore Rules এই project-এর `firestore.rules` ফাইলে দেওয়া আছে।

## Important
Firestore Rules access control/data validation করে; browser-এর client code নিজে trusted payment verifier নয়। Order amount/stock/payment verification-এর মতো sensitive business checks production-এ server-side validation দিয়ে আরও শক্ত করা যায়.

## Deploy
Netlify Drop বা Vercel-এ এই folder/ZIP-এর files deploy করো।
