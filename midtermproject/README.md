# MIDTERM PROJECT
For this assignment first I began using the code that we all wrote / read together in class. The code structure is found inside the "05Functions" folder of the class repository.
## code reference
[Code Reference](https://github.com/rdwrome/261sp25/blob/main/05Functions/codealong.js)
#### notes
The first thing I did was to add more sound to the code. I began by writing let mysecondsound and third sound but then realized I also needed to specify the sounds in the preload area:

```
let myFirstSound;
let mySecondSound;
let myThirdSound;
```
Then, I loaded the samples and specified their name and location: 

```
function preload() {
  soundFormats('wav', 'mp3');  
  mySecondSound = loadSound('trumpet 0008 [2025-02-25 204828].wav', soundLoaded);
  myFirstSound = loadSound('sax 0001 [2025-02-25 203029].wav')
  myThirdSound = loadSound('trpm.wav')
}
```
After that I decided which keys I wanted to use and went ahead and wrote the code for them
In this part of the process I began by trying the function if for each specific key, but realized I needed to use the function "else if":

```
function keyPressed() {
  console.log("Key pressed:", key);
  if (key.toLowerCase() === 'o') {
    playCustomSound(mySecondSound);
  } 
  else if (key.toLowerCase() === 'p'){
    playCustomSound(myFirstSound);
  }
    else if (key.toLowerCase() === 'i'){
    playCustomSound(myThirdSound);
    }
```
	
Apart from that, the process was straight forward.

#### midterm 
[MIDTERM PROJECT](https://editor.p5js.org/lcurik/sketches/J94HsnvXg)