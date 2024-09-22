this is a MATLAB package, which increase the speed of PsychToolbox devlopment and decrease bug.

add `+PTB` folder path to MATLAB search path to install

## example

```matlab
app = PTB.App(); % build app
app.debug(); % debug mode
app.backgroundColor = [255 255 255];
app.begin(); % run app
app.Element.multiText('welcome to test task\npress space key to start'); % draw muti-lines text
app.Element.render(inf); % render texture, and listen keyboard
app.finish(); % end app
```

## todo

refactor to MVVM architecture
