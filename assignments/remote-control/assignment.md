# Assignment: Remote Control

## Description

Your task is to implement remote control backend using RobotJS library and websocket.

The backend should be able to do the following:

- Start websocket server
- Handle websocket connection
- Move mouse (Up, Down, Left, Right)
- Draw circle, rectangle and square  
- Send current mouse coordinates
- Send desktop capture

## Technical requirements

- Only [ws](https://www.npmjs.com/package/ws) and [robotjs](https://www.npmjs.com/package/robotjs) dependencies and subdependencies should be required
- The program is started by npm-script start in following way:
npm run start 
- After starting the program displays websocket parameters
- After program work finished the program should end websocket work correctly  
- After each received command program should display the command and result
- All commands should be ended with **\0**

List of websocket commands and their syntax:
- Navigation
    - Move mouse up
    ```bash
    mouse_up
    ```
    - Move mouse down
    ```bash
    mouse_down
    ```
    - Move mouse left
    ```bash
    mouse_left
    ```
    - Move mouse right
    ```bash
    mouse_right
    ```
    - Send mouse coordinates
    ```bash
    mouse_right
    ```
- Drawing
    - Draw circle with pushed left button: 
    ```bash
    draw_circle
    ```
    - Draw rectangle with pushed left button: 
    ```bash
    draw_rectangle
    ```
    - Draw square with pushed left button: 
    ```bash
    draw_square
    ```
- Print screen
    - Make print screen command and send image:
    ```bash
    prnt_scrn
    ```
    