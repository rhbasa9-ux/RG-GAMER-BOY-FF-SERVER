RG GAMER BOY FF — deployment package

Two separate deployments are included. Do not merge Firebase code into the Winter website.

GOOGLE LOGIN: Upload the contents of google-login-system/ to the root of a separate GitHub Pages repository for the login site. Firebase config uses the latest supplied project rg-gamer-boy-ff-login. In Firebase Console for that project, enable Google under Authentication, add the deployed login hostname under Authentication > Settings > Authorized domains, and publish google-login-system/database.rules.json to Realtime Database.

After Google sign-in, Continue opens https://rggamerboyff.github.io/RG-GAMER-BOY-FF/. Delete Account opens the Google Form URL already included in the supplied ZIP. It submits a deletion request and does not instantly delete the account. The username/password option opens the same existing website URL.

WINTER WEBSITE: winter-website/index.html is the uploaded Winter Special index, copied unchanged. It has no Firebase SDK connection and retains its existing CAPTCHA and winter music code. The audio element expects swiat_rafika-peaceful-winter-night-soft-ambient-snowy-atmosphere-448985.mp3 in the same GitHub Pages folder as this index.html. Upload that MP3 directly to the root of the Winter website repository with exactly that filename.

PING DISPLAY: Region Ping measures a round-trip response to the configured Firebase Realtime Database endpoint every 10 seconds. Network Estimate displays the browser-provided connection downlink estimate in Mbps; it is not a measured download speed, and some browsers do not expose this API.

LIMIT: Static code checks do not prove live OAuth/database success. After deployment, test on HTTPS and confirm Google is enabled, the login domain is authorized, and the rules are published to the rg-gamer-boy-ff-login project.
