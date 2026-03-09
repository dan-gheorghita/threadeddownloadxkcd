# threadedDownloadXkcd.py

**Multithreaded XKCD Comic Downloader**

This Python script, `multidownloadXkcd.py`, is designed to download XKCD comics using multiple threads. It creates and starts 14 threads, each responsible for downloading a batch of 10 comics from the XKCD website.

**Functionality**

The script uses the following libraries:

1. `requests`: For making HTTP requests to the XKCD website.
2. `bs4` (BeautifulSoup): For parsing the HTML content of the web pages.
3. `threading`: For creating and managing multiple threads.
4. `os`: For creating directories and joining file paths.

Here's a step-by-step breakdown of the script's functionality:

1. **Directory creation**: The script creates a directory named `xkcd` in the current working directory, if it doesn't already exist.
2. **`downloadXkcd` function**: This function takes two arguments, `startComic` and `endComic`,