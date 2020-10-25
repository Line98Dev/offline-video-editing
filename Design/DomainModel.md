![The Domain Model](https://raw.githubusercontent.com/Line98Dev/offline-video-editing/master/Design/DomainModel.png)

### User
- Name (String): The name of the user.
- Email (String): The email address of the user.
- Videos (List<Video>): The list of videos this user has uploaded.
- Type (String): The type of the account of the user (what features are available to them).
- Sports (List<Sports>): The list of sports the user has added to their account (including level).

### Sport
- Type (String): The type of sport the user added.
- Level (String): The level of skill of the user.

### Video
- Length (Integer): The length of the video.
- Date (Date): The date/timestamp of the video.
- Content (List<Content>): The list of content added to the video (like slides, voiceover, telestration, tag, and polls).
- HomeTeam (String): The name of the home team which played.
- AwayTeam (String): The name of the away team which played.
- Game (Integer): The game number of the video.
- Title (String): The title of the video.
- Sport (String): Which sport which was played.
- Level (String): The skill level of he event (middle school, high school, collegiate, etc.).
- Location (String): Where the event took place.
- Description (String): The description of the video/event.

### Content
- Timestamp (Integer): The spot in which the content starts.
- Creation Date (Date): The date which the content was created.
- Video (Video): The video which includes the content.
- Author (User): The person who created the content.
- Length (Integer): The length the content displays.

### Slide (implements Content)
- Message (String): The message to show during the video.

### Poll (implements Content)
- Options (Array<String>): A array of selections for the poll.
- Answer (Integer): The index of the Options array which is the correct option.
- Closing Time (Date): The date & time which the poll closes.

### Voiceover (implements Content)
- Audio (Audio): The audio file of the voiceover.
- Title (String): The title of the voiceover.
- Description (String): The description of the voiceover (or captions).

### Teletration (implements Content)
- Name (String): The name of the telestration.
- Type (String): The type of the telestration (line, square, circle, custom, etc.).
- Color (String): The color of the telestration.
- X & Y (Integers): The coordinates (x and y respectively) where the telestration is.
