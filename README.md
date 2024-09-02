# A multi platform simple devcontainer template

## Requirements
- [Docker](https://docs.docker.com/get-started/get-docker/)
- [VSCode](https://code.visualstudio.com/)
- VScode Extensions:
    - [Remote Development](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack)

## Modes
- Linux Mode
    - Works in all GNU/linux os which uses either x11 or Wayland windowing methods.
- Windows
    - Works in all windows os with Windows Subsystem for Linux(WSL) installed.
        <img src="https://github.com/user-attachments/assets/4f8ab803-5978-4b84-a8ca-2ca341396634" alt="Image Description" width="600" height="300">
- Universal
    - Works in linux, windows, macos, etc.. with docker engine installed.
 
## Usage
- Clone the repository
```
git clone https://github.com/manojm-dev/simple_ros_devcontainer rosdev_ws
```
- Open the folder in vscode
  
    - Terminal Method
      ```
      cd rosdev_ws
      ```
    - GUI Method
      Open vscode then `File > Open Folder (Ctrl + O)` and open the folder.
      
- Opening the devconaintainer 
    - **Method 1:** 
        -  Click reopen  in devcontainer button
        ![image](https://github.com/user-attachments/assets/978a1d14-2f91-4e80-98cd-2587d7c0a5ff)
        
        - Choose the option you want
        ![2](https://github.com/user-attachments/assets/68cd1ba3-5648-48c9-bfd1-bb05191c14a3)
      
    - **Method 2:**
        - Press `Ctrl + Shift + P` and search `rebuild` and click the `Dev Containers: Rebuild and Reopen in Container` option
        ![1](https://github.com/user-attachments/assets/099a17f4-e792-4a1f-8f70-ceef54450ce3)

        - Choose the option you want
        ![2](https://github.com/user-attachments/assets/68cd1ba3-5648-48c9-bfd1-bb05191c14a3)



