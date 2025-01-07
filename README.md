# Youtube-video-downloader
1. Tk() – The Tk() method helps us create a blank GUI Window.

2. geometry() – The geometry() method defines the size of the GUI Window.

3. Title – The title() method gives an appropriate title to the GUI Window.

4. Label() -The label() method creates a widget on the GUI Window which helps us display a piece of text. You can specify the following attributes inside a Label() method:

Text – what text to be displayed.
Bg – Background colour.
Fg- Foreground colour.
Font – The font of the text
5. Entry() – The Entry() method helps us create an entry field on the GUI Window. We can specify the following things inside the Entry() method:

Width – The width of the entry field.
Textvariable – what variable will be associated with the entry field.
6. Checkbutton() – The CheckButton() method creates check buttons on the GUI Window. For one checkbutton the method is used one. Inside a checkbutton() method, we can specify the following things:

Onvalue – The value assigned when the check button is checked.
Text – The text visible with the checkbutton.
Textvariable – The variable associated with the checkbutton.
7. Button() – The button() method helps us create a Button on the GUI Window. Inside a Button() method, we can specify the following attributes:

Text – Text on the button.
Command – The function to be evoked when the button is clicked.
Bg – Colour of the button.
Fg – Foreground colour.
8. pack() – pack function s to display all the widgets on the GUI Window.

 
    video_streams = video.streams.filter(file_extension = 'mp4').get_by_itag(res)
    video_streams.download(filename = "Untitled", output_path = "video_path")
    Label(window,text="Downloaded Successfully").pack()
We have created the downloader function to download a video from YouTube.
We have created a global variable res.
get() – Using the get() method, we get the value entered in the entry field.
YouTube() – Extracts the video from YouTube.
video.streams.filter() – Is to set the filter to the video.
get_by_itag() – Is to specify the resolution of the video.
download() – Is to download the video.
