Download the file from the service URL.

Open Firefox (or the browser of your choice) and load the SharePoint page with the video that you want to download, then open the page inspector (Ctrl + Shift + C). Click on the Network tab. Type videomanifest where it says “Filter URLs“. Press F5 to refresh the page. When the page reloads, copy the file URL. See below.

  ![image](https://github.com/ObsidianMaximus/optix/assets/97427045/1fe2c171-382d-4faf-8346-feed67372c30)

Use ffmpeg to download the video by pasting the URL from above:

# $ ffmpeg -i "https://copied_videomanifest_url" -codec copy video.mp4


Source : https://www.lisenet.com/2022/how-to-download-view-only-teams-meeting-recording-video-from-sharepoint/
