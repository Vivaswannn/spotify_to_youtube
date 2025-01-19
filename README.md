# SpotifyToYoutubeMP3

SpotifyToYoutubeMP3 is a Python-based application that allows users to download their Spotify playlists or saved tracks as MP3 files by fetching the audio from YouTube. It combines the power of the Spotify API and YouTube APIs to provide a seamless experience.

## Features
- Authenticate using Spotify's OAuth 2.0.
- Retrieve and display saved tracks or playlists from your Spotify account.
- Map Spotify tracks to corresponding YouTube videos.
- Download audio from YouTube in MP3 format.
- User-friendly web interface powered by Flask.

## Tech Stack
- **Backend:** Python, Flask
- **APIs:** Spotify API, YouTube
- **Libraries:**
  - Spotipy: For interacting with Spotify API
  - youtube_dl: For downloading audio from YouTube
  - Flask: For creating the web application

## Requirements
- Python 3.6+
- Spotify Developer Account
- Internet connection

## Installation

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/<your-username>/SpotifyToYoutubeMP3.git
   cd SpotifyToYoutubeMP3
   ```

2. **Create a Virtual Environment (Optional but Recommended):**
   ```bash
   python -m venv venv
   source venv/bin/activate      # On macOS/Linux
   .\venv\Scripts\activate     # On Windows
   ```

3. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Set Up Spotify API Credentials:**
   - Go to the [Spotify Developer Dashboard](https://developer.spotify.com/dashboard/).
   - Create a new app and note down the **Client ID** and **Client Secret**.
   - Add a Redirect URI (e.g., `http://127.0.0.1:5000/redirect`).

5. **Update `app.py`:**
   Replace placeholders with your Spotify credentials:
   ```python
   client_id = "YOUR_CLIENT_ID"
   client_secret = "YOUR_CLIENT_SECRET"
   redirect_uri = "http://127.0.0.1:5000/redirect"
   ```

## Usage

1. **Run the Application:**
   ```bash
   python app.py
   ```

2. **Open in Browser:**
   Navigate to `http://127.0.0.1:5000/`.

3. **Login to Spotify:**
   - Authenticate using your Spotify account.

4. **Download MP3s:**
   - The app fetches your saved tracks and downloads corresponding MP3 files from YouTube.

## Potential Improvements
- Enhance the UI/UX of the web interface.
- Optimize playlist handling for large playlists using multi-threading.
- Add support for saving MP3 files directly to cloud storage (e.g., Google Drive).
- Implement better error handling for missing tracks or API rate limits.

## License
This project is licensed under the MIT License. See the LICENSE file for more details.

## Contributing
Contributions are welcome! Feel free to fork this repository and submit a pull request.

---

Feel free to reach out with any questions or feedback!
