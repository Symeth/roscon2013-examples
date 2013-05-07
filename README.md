# ROSCon 2013 Robot Web Tool Examples

## About

[ROSCon](http://roscon.ros.org/) is a conference covering the [Robot Operating
System](http://www.ros.org)(ROS), an open-source robot framework.

At ROSCon 2013, I gave a presentation showing how to make web apps for robots,
using libraries from the [Robot Web Tools](http://robotwebtools.org/)
community. The examples of that presentation range from connecting to a
ROS-enabled robot from a web browser all the way to rendering a robot in 3D
inside a browser.

This repo includes all the example code shown during the presentation.

## How to Run

The demos were done with a [TurtleBot
2](http://store.iheartengineering.com/ihe-2700-000c-0000.html). However, the
fundamentals should work with any robot, and most of the examples can be run on
just a computer running ROS. No robot required!

To run:

 1. [Install ROS](http://www.ros.org/wiki/ROS/Installation). I recommend using
  Ubuntu or a VM running Ubuntu 12.04+. If an absolute beginner to ROS, the
  [docs on ros.org](http://www.ros.org/wiki/ROS/Introduction) are very well done,
  as is this [Getting
  Started](http://spectrum.ieee.org/tag/turtlebot%20tutorial/?media=all&max=10&offset=0&sortby=desc)
  series on the IEEE Spectrum blog.

 2. Install the dependencies for the examples. The
  ros/installRosDependencies.sh script will install all the necessary deb
  packages.

  ```bash
  sudo apt-get install ./ros/installRosDependencies.sh
  ```

 3. Run a local web server. Luckily, this doesn't require Apache, just running
  out-of-the-box Python:

  ```bash
  python -m SimpleHTTPServer
  ```

 4. Visit the web page. Go to http://localhost:8000/step0.html to see the first
  example. Then http://localhost:8000/step1.html for the next example, and so
  on!

## License (BSD)

```
Copyright (c) 2013, Brandon Ace Alexander
All rights reserved.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:

Redistributions of source code must retain the above copyright notice, this
list of conditions and the following disclaimer.

Redistributions in binary form must reproduce the above copyright notice, this
list of conditions and the following disclaimer in the documentation and/or
other materials provided with the distribution.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```
