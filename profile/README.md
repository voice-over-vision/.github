<!-- header -->
<div align="center" style="margin-bottom:20px">
    <img src="https://github.com/voice-over-vision/.github/blob/main/assets/logo_banner.png?raw=true"/>
</div>

<!-- content -->
<p align="center">
 <a href="#🎬-demos">Demos</a> •
 <a href="#🚀-features">Features</a> •
 <a href="#💻-installation">Installation</a> •
 <a href="#🌟-contribution">Contribution</a> • 
 <a href="#💎-acknowledgments">Acknowledgments</a> • 
 <a href="#📄-citation">Citation</a>
</p>

<!-- intro -->

## Voice-Over Vision: The future of the internet is accessible

We present **Voice-Over Vision**, a tool that transforms YouTube watching for the visually impaired, making every video more accessible and enjoyable. Like a friend sitting next to you, this Chrome Extension narrates the unseen parts of a video, filling in the blanks where audio alone falls short. It smartly sifts through videos, picking out details that you might miss otherwise, and uses text-to-speech technology to bring those visuals to life through vivid descriptions. With Voice-Over Vision, every story is fully told, ensuring everyone gets the complete picture, no matter what.

<!-- demos -->

## 🎬 Demos

[![Voice-Over Video Demo](https://img.youtube.com/vi/6-y6Nq-UWZw/0.jpg)](https://www.youtube.com/watch?v=6-y6Nq-UWZw)

<!-- features -->

## 🚀 Features

- **Real-Time Audio Description**: Generates audio descriptions for YouTube videos, offering a comprehensive viewing experience for visually impaired users.
- **Ask The Video**: Answers questions about the video at any time. With just the click of a button (or a keyboard shortcut), the video pauses and a chat opens to clarify any and all questions about the video!
- **More coming soon!**

<details>
<summary>Work In Progress</summary>

- [ ] **Customizable Speech Parameters**: Adjust voice selection, speech rate, and volume to tailor the audio descriptions to your preferences.
- [ ] **Detail Level Settings**: Choose the level of detail for descriptions, from basic overviews to in-depth analysis of physical appearances and emotions.
- [ ] **Interruption Frequency Control**: Select how often you'd like the video's original audio to be interrupted with descriptions, ensuring a balanced experience.
</details>

<!-- installation -->

## 💻 Installation

Instructions on how to install and run Voice-Over Vision (soon to be released at Google Chrome Extensions marketplace)

<!-- prerequisites -->

### Prerequisites

- Google Chrome or any Chromium-based browser (except for Brave, for now).
- Git installed and configured on your machine
- Python version: 3.11.8
- Pip: 24.0

<!-- installation_backend -->

### Installing the back-end

#### 1. **Clone the repository**:

```sh
git clone https://github.com/voice-over-vision/vov-backend.git
cd vov-backend
```

#### 2. **Install dependencies**

```sh
# Create a virtual environment and activate it

## Linux
python3 -m venv env
source env/bin/activate

## Windows
python -m venv env
env\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

#### 3. **Configure the OpenAI key**

```sh
# Change directories into the vov_backend app
cd vov_backend

# Create an environment file

# Linux
touch .env

# Windows
cd . > .env
```

- The .env file sould contain

```sh
OPENAI_API_KEY={OPENAI_API_KEY} # OPENAI_API_KEY should be replaced by your API_KEY from OpenAI
```

#### 4. **Run the server**

```sh
cd ../ # return to the project's root directory
python manage.py runserver
```

- You can test the backend by navegating to [http://127.0.0.1:8000/get_audio_description?youtubeID=keOaQm6RpBg](http://127.0.0.1:8000/get_audio_description?youtubeID=keOaQm6RpBg)

<!-- installation_frontend -->

### Installing the Chrome Extension

#### 1. **Clone the repository**:

```
git clone https://github.com/voice-over-vision/vov-chrome-extension.git
```

#### 2. **Load the extension in Chrome** (detailed information [here](https://developer.chrome.com/docs/extensions/get-started/tutorial/hello-world#load-unpacked)):

- Open the _Manage Extensions_ page by navigating to `chrome://extensions/` in your Chrome browser.
  <br/><br/>
  <img src="https://github.com/voice-over-vision/.github/blob/main/assets/chrome_ext_domain.png?raw=true" width="380px"/>
  <br/><br/>
- Enable _Developer mode_ by toggling the switch at the top-right corner.
  <br/><br/>
  <img src="https://github.com/voice-over-vision/.github/blob/main/assets/chrome_dev_mode.png?raw=true" width="220px"/>
  <br/><br/>
- Click on _Load unpacked_ and select the directory of your cloned repository.
  <br/><br/>
  <img src="https://github.com/voice-over-vision/.github/blob/main/assets/chrome_load_ext.png?raw=true" width="280px"/>
  <br/><br/>
- The extension should now be installed and visible in your Extensions list, you can pin it if you want by clicking the Pin icon.
  <br/><br/>
  <img src="https://github.com/voice-over-vision/.github/blob/main/assets/chrome_pin_ext.png?raw=true" width="280px"/>
  <br/><br/>

#### 3. Enjoy the magic of Voice-Over Video!✨

<!-- contribution -->

## 🌟 Contribution

<table>
  <tbody>
    <tr>
      <td align="center" valign="top" width=15%>
        <a href="https://github.com/DaviGiordano" style="text-decoration: none;">
          <img src="https://github.com/DaviGiordano.png" width="100%;" style="max-width:150px" alt="Davi Giordano"/>
          <br/>
          <sub><b>Davi Giordano</b></sub>
        </a>
      </td>
      <td align="center" valign="top" width=15%>
        <a href="https://github.com/guilherme-francisco" style="text-decoration: none;">
          <img src="https://github.com/guilherme-francisco.png" width="100%;" style="max-width:150px"alt="Guilherme Mariano"/>
          <br />
          <sub><b>Guilherme Mariano</b></sub>
        </a>
      </td>
      <td align="center" valign="top" width=15%>
        <a href="https://github.com/marianaserrao" style="text-decoration: none;">
          <img src="https://github.com/marianaserrao.png" width="100%;" style="max-width:150px" alt="Mariana Serrao"/>
          <br />
          <sub><b>Mariana Serrão</b></sub>
        </a>
      </td>
      <td align="center" valign="top" width=15%>
        <a href="https://github.com/murillo-teixeira" style="text-decoration: none;">
          <img src="https://github.com/murillo-teixeira.png" width="100%;" style="max-width:150px" alt="Murillo Teixeira"/>
          <br />
          <sub><b>Murillo Teixeira</b></sub>
        </a>
      </td>
    </tr>
  </tbody>
</table>

<!-- acknowledgments -->

## 💎 Acknowledgments

### Chroma DB

We extend our heartfelt thanks to the developers and community behind Chroma DB for their exceptional AI-native open-source embedding database, a crucial component in our mission to create an accessibility tool for the visually impaired. ChromaDB's robust and efficient data management capabilities have been pivotal in our efforts to make a positive impact.

### GPT-4

Our appreciation goes to the OpenAI team for providing foundational AI technology for our project. The robustness of GPT-4 was instrumental in our project's natural language processing and image processing capabilities.

<!-- citation -->

## 📄 Citation

```bibtex
@software{voice-over-vision,
  author = {Davi Giordano, Guilherme Mariano, Mariana Serrao and Murillo Teixeira},
  title = {Voice-Over Vision: The future of the internet is accessible},
  month = {March},
  year = {2024},
  url = {https://github.com/voice-over-vision}
}
```
