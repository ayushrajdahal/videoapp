## File Storage Backend made using Fast API

Instructions to run this on your computer:

1. `git clone https://github.com/ayushrajdahal/videoapp`
2. `pip install -r requirements.txt`.
3. `python3 videoproject.py` or `uvicorn videoproject:app --reload`

**API Endpoints:**

1. `/upload-video` recieves and validates the video file

2. `/list-videos` lists videos that satisfy the conditions passed (all are optional)
    - **minLength:** minimum video length in seconds
    - **maxLength:** maximum video length in seconds
    - **dateFrom:** earliest date in 'YYYY-MM-DD'
    - **dateTill:** latest date in 'YYYY-MM-DD'

3. `/calculate-charges` calculates total charge, given the video size, length, and file type via Query Parameters

4. `/stream-video` streams stored video, given the filename as an input

To access the API Documentation page, go to http://127.0.0.1:5000/docs