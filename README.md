# BI Help Bot Improvement

This project aims to enhance the BI Help Bot on Slack to better answer questions related to Superset. The improvements include integrating voice-to-text from a YouTube channel and web scraping from the official Superset blog.

## Objective

To improve the BI Help Bot on Slack by:
1. Implementing a voice-to-text feature from the YouTube channel `@preset`.
2. Extracting data from blog posts on the official Superset website.

## Project Structure

The project consists of two main scripts:
1. `Youtube_to_text.ipynb`: Converts voice to text from the YouTube channel `@preset`.
2. `Webscraping_Preset_Blog.ipynb`: Extracts data from blog posts on the official Superset website.

## Files

- `Youtube_to_text.ipynb`: Jupyter notebook containing the script for voice-to-text conversion from YouTube videos.
- `Webscraping_Preset_Blog.ipynb`: Jupyter notebook containing the script for web scraping the official Superset blog.

## Prerequisites

Before running the scripts, ensure you have the following installed:
- Python 3.7 or later
- Jupyter Notebook
- Required Python packages (listed in each notebook)

## Setup and Usage

### Voice-to-Text Conversion

The `Youtube_to_text.ipynb` notebook converts audio from YouTube videos to text. Here's a detailed explanation of the code:

1. **Import Libraries**: The script imports necessary libraries such as `pytube` for downloading YouTube videos and `speech_recognition` for converting speech to text.
   
2. **Download Video**: Using `pytube`, the script downloads a video from the YouTube channel `@preset` specified by its URL.

3. **Extract Audio**: The script extracts audio from the downloaded video file using `moviepy.editor`.

4. **Convert Speech to Text**: With the `speech_recognition` library, the script converts the extracted audio to text. It splits the audio into smaller segments for more accurate recognition.

5. **Output**: The converted text is then outputted and can be saved or processed further.

### Web Scraping from Superset Blog

The `Webscraping_Preset_Blog.ipynb` notebook extracts data from the official Superset blog. Here's a detailed explanation of the code:

1. **Import Libraries**: The script imports libraries such as `requests` for sending HTTP requests and `BeautifulSoup` for parsing HTML content.

2. **Fetch Blog Content**: The script sends a request to the Superset blog URL and retrieves the HTML content of the blog page.

3. **Parse HTML**: Using `BeautifulSoup`, the script parses the HTML content to identify and extract specific elements such as blog post titles, dates, and content.

4. **Data Extraction**: The script iterates through the parsed HTML, extracting relevant information from each blog post.

5. **Output**: The extracted data is then outputted in a structured format (e.g., a DataFrame) for further use or analysis.


## Contact

For any questions or support, please contact [penpitcha.siriwan@agoda.com],[siroros.roongdonsai@agoda.com],[yanisa.treesak@agoda.com],.

---

**Note:** Ensure you have the appropriate permissions to use the data from the YouTube channel and the official Superset blog for this project.
