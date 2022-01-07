[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-f059dc9a6f8d3a56e377f745f24479a46679e63a5d9fe6f495e02850cd0d8118.svg)](https://classroom.github.com/online_ide?assignment_repo_id=6647448&assignment_repo_type=AssignmentRepo)
# Processing Task 5 - Input

## Learning Objectives
In this task, you will learn about:
* Mouse Input
  * The `mouseX` and `mouseY` Variables
  * The `mousePressed` Variable
  * Mouse Input Functions
  * Combining Input Variables and Event Functions
* Keyboard Input
  * The `keyPressed` Variable
  * The `key` Variable
  * The `keyCode` Variable
  * Keyboard Input Functions
  * Handling Multiple Keys


## Step 1 - Lesson
Acquire the learning objectives by reviewing [this page from Happycoding.io](https://happycoding.io/tutorials/processing/input)

## Step 2 - Task
Create a drawing program for a specific scene. For example, you could create a garden drawing program where clicking creates flowers (randomly sized and colored?), dragging creates grass, the mouse wheel adds butterflies, keyboard changes the background or sky.  You can re-use functions from previous tasks defined to draw items to the screen (i.e flowers, clouds, etc).  The objective is to demonstrate your ability to do as many of the lesson learning objectives as possible.  

## Evaluation 
### Level 2
Demonstrates 2 - 4 learning objectives

### Level 3
Demonstrates 5 - 7 learning objectives

### Level 4
Demonstrates > 7 learning objectives



## Submission
1. Commit and push your code to this repository
2. Record a screen recording video demonstrating your drawing program.  Submit it to the Google Classroom Assignment post.
3. Take a screenshot of your work and upload it to the Google Classroom assignment post
4. In the google doc attached to the assignment, complete the Learning Objectives checklist by adding a brief description about how you demonstrated the learning objective (1-2 lines).

import processing.core.PApplet;

public class Sketch extends PApplet {
	
  public void settings() {
	// put your size call here
    size(500, 500);
  }

  public void setup() {   
  }
  
  public void mouseDragged() {
      
    stroke(89, 143, 74);
    fill(89, 143, 74);
    ellipse(mouseX, mouseY, 100, 100);

  }

  public void mouseClicked() {

    stroke(255, 209, 233);
    fill(255, 209, 233);
    ellipse(200, 200, 100, 100);
    ellipse(300, 200, 100, 100);
    ellipse(200, 300, 100, 100);
    ellipse(300, 300, 100, 100);
    stroke(255, 242, 158);
    fill(2255, 242, 158);
    ellipse(250, 250, 100, 100);
    
  }

  public void draw() {

    if (keyPressed) {
      background(153, 228, 255);
    }else if (key == 's') {
      stroke(252, 239, 119);
      fill(252, 239, 119);
      ellipse(30, 30, 150, 150);
    }else if (keyCode == UP) {
      stroke(255, 255, 255);
      fill(255, 255, 255);
      ellipse(400, 120, 50, 50);
      ellipse(360, 120, 50, 50);
      ellipse(320, 120, 50, 50);
      ellipse(280, 120, 50, 50);
      ellipse(380, 90, 50, 50);
      ellipse(340, 90, 50, 50);
      ellipse(300, 90, 50, 50);
      ellipse(340, 70, 75, 75);
    }
  }
}
