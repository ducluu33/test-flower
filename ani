function setup() {
  createCanvas(windowWidth, windowHeight);
  background(0);  // Set background color to black
  stroke(139, 69, 19); // Brown color for tree branches
  translate(width / 2, height); // Start at the bottom center
  branch(100);  // Initial branch length
}

function branch(len) {
  strokeWeight(2);
  if (len > 10) {
    // Draw the branch
    line(0, 0, 0, -len);
    translate(0, -len);
    
    // Recursive calls
    push(); // Save current drawing state
    rotate(PI / 6); // Rotate by 30 degrees
    branch(len * 0.75); // Shorten and draw the next branch
    pop();  // Restore previous drawing state
    
    push();
    rotate(-PI / 6); // Rotate by -30 degrees
    branch(len * 0.75); 
    pop();
  } else {
    // Draw leaves
    fill(255, 165, 0); // Orange color for leaves
    ellipse(0, 0, 10, 10);
  }
}
