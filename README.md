# JOHTnotes
> Tip: Pronounced _"jot notes"_ with a silent 'h'

![gallery](https://user-images.githubusercontent.com/68176295/136850663-e5d1247f-83d8-4892-a72a-85c1b5280dfe.jpg)

_Video library_

![gallery (1)](https://user-images.githubusercontent.com/68176295/136850670-45ae021e-64b5-4699-bde1-366ca8de6e4f.jpg)

_Taking Notes!!_

## Inspiration
Ever wondered if you can quickly jump to the topic you want in a long lecture (_ewww_)? What about linking up your notes to a specific timestamp so you can quickly find the context? During this period of global pandemic, millions of students of all ages are confined to learning online, spending hours per day listening to lectures, tutorials, and labs. We hope that our project will make this experience smoother and more productive for students, whether studying from Jamaica or Canada. 

## What it does
JOTHnotes is a web platform where students can import and watch lecture videos, while also being able to make notes at timestamps within the videos. In addition, with a readily available transcript created upon each video upload, users can search and filter keywords/phrases spoken by the teacher. Every video timestamp can be clicked to skip to the respective section, offering a more intuitive experience for the student.

## How we built it
Our project began with each component set up separately:
* designed a basic static web interface with HTML, CSS, JavaScript, and React to experiment with layout
* developed a Flask REST API template in Python
* configured a connection to Google Cloud Storage for storing video, audio, and thumbnail files
* implemented the Google Cloud Speech-to-Text API to generate a transcript from audio data 
set up a CockroachDB relational database for manipulating video metadata, annotations, and transcripts

Once we had our foundation laid out, we worked on integrating the important backend functionalities into the Flask API. Meanwhile, on the frontend, we added more interactive page components and improved the appearance.
After testing and fixing the bugs in our code, we redesigned the interface for a cleaner aesthetic. With everything ready, we containerized the backend and hosted it on Google Cloud Run. 

## Challenges we ran into
* Deploying to the cloud
* A member of our group was not able to run React locally and had to work with Repl.it. Working with version control and transferring changes across the two systems was a big pain  

## Accomplishments that we're proud of
As a team with three first-time hackers, we are proud of the teamwork and camaraderie developed during the past days. In fact, “JOHT” is composed of the first letter of our names! We are also very proud of JOHTnotes, which is all that we expected it to be and a little more. We are excited to see how it might help real users in the future!

## What we learned
Dream big, work hard, code for a purpose one line at a time.

## What's next for JOHTnotes
Transcript translation into different languages for even greater accessibility! We also want to implement one-click download, where notes and transcripts are saved neatly into one downloadable PDF. Other things on the roadmap include: 
* Implement a user login system for a personalized experience and also introduce a general feed where you can have access to various lectures and videos.
* Add a folder/flair system to organize lectures by courses
* Optimize the transcript generation function to decrease wait time

