# Complete-Application
This repository contains all three components of our mission smile application. The application can evaluate the emotion of the user and would give a corresponding recommendation what the user should do.

## Structure
- The folder docs contains all our [documentation folder](/docs/)
- Here is our [documentation file](/docs/Dokumentation_MissionSmile.pdf)
- Here is our grade distribution [grade](/docs/Notenverteilung_MissionSmile.pdf)
- Here is our [presentation folder](/docs/presentations/)
- The folder Emotion-Recognition-API contains our [emotion recognition application folder](/Emotion-Recognition-API/)
- The folder Recommendation-API contains our [Recommendation application folder](/Recommendation-API/)
- The folder frontend contains our [frontend](/frontend/)
## See our application directly
All of our services and application are deployed on Vercel and Heroku. First request to the application could be slow, since the application will go to sleep, when the application doesn't receive any traffic in one hour. Any subsequent requests will perform normally through.
To wake up our backend-APIs, please click on these links below:
- wake up Recommendation-API: https://smile-emotion-recognition.herokuapp.com/helloWorld
- wake up Emotion-Recognition-API: https://powerful-plains-46454.herokuapp.com/helloWorld

This could take up to one minute, until the services are active. If it didn't, just refresh the website. <br>
After waking up the application, you can go to our frontend under this link: https://mission-smile.vercel.app/

## Start the application locally
start <strong>Emotion-Recognition-API</strong>

```
cd Emotion-Recognition-API
pip install -r requirements.txt
python app.py
```
If it doesn't work, you could use Docker to start the image. Just uncomment the penultimate line and comment the last line out.

start <strong>Recommendation-API</strong>
```
cd Recommendation-API
pip install -r requirements.txt
python app.py
```

start <strong>frontend</strong>
```
cd frontend
npm install
npm run dev
```
After that go to [pages/index.js](/frontend/) and replace the value of const url_emo with the localhost port where the emotion-recognition service is running. Also replace the value of const url_recom_base with the localhost port of the recommendation-api.

## Remarks
Our application were developed on different repositories. This repository contains just the end result. To see our development reposities follow those links:
- frontend: https://github.com/bila9630/MissionSmile
- Recommendation-API: https://github.com/Mission-Smile/Recommendation-API
- Emotion-Recognition-API: https://github.com/Mission-Smile/Emotion-Recognition-API