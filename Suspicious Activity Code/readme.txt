>application directory has contents of saved model and flask API connection to run it as web application for prediction.
>codes directory has contents of colab files which were used for creating 2 models(.pynb files)
----------------------------------------------------------------------------------------------------------

STEPS FOR EXECUTING APPLICATION:

1. Extract the application folder in your machine.
2. unsus_keras.pb is the directory of saved model.
3. ~/application/Flask/static/files/frames=> stores the image files(frames) from the uploaded video.
4. Inside main.py, change the directory for load_model as per your own machine
5. Run main.py python file.Then you will get the url for the app.
6. open the browser and hit the url so that home page will be displayed.
7. Click the add-file buttton and upload the video which needs to be given as input to model.
8. Then click on submit button. 
9. After Clicking submit button, you will be redirected to result page in which the
   type of suspicious activity occured in that video will be displayed after prediction from model.