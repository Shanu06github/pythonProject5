

                                                                                    Ice Cream Haven

Description:
Ice Cream Haven is a desktop application built using Python and Tkinter for a virtual ice cream parlor. Customers can view available flavors, suggest new flavors, add flavors to their cart, and view their cart.

Features
-->View available ice cream flavors
-->Search for specific flavors
-->Add flavors to cart with optional notes
-->View cart with selected flavors and notes
-->Suggest new ice cream flavors

To run this Project:

->Clone this project in your terminal 
->Download the docker file that is uploaded and run it in your terminal using the following commands

COMMAND:1
-->docker build -t icecream-parlor-app .
After successful building of the application ,you have to download a X-server for viewing a GUI based application using docker that is Xming is used for my project which is easy to download and setup and after that run the following command in terminal

COMMAND :2
-->docker run -it --rm -e DISPLAY=host.docker.internal:0 -v C:/tmp/.X11-unix:/tmp/.X11-unix -v images:/app/images icecream-parlor-app

images:/app/images-->if this did not work change this path to the images path

If this command shows any error after running in the terminal, please create a file in the xming directory called  'X0.hosts' in that file give localhost and save it and then run the same command and it should run.