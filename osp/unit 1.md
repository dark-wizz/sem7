# Introduction to Open Source

---

- Open Sources
  - Need
  - Advantages
  - Application
- Open source operating systems: LINUX
  - Introduction
  - General overview
  - Kernel mode and user mode Process
  - Scheduling
  - Personalities Cloning Signals
  - Development with Linux.

---

### Part A

- [ ] What is GNU(GPL)?
  > [!info]- Ans
  > GNU(GNU's Not Unix) is a Unix like operating system that are free and open source
  > GNU GPL(General Public License) is a free, copyleft license for softwares and other kinds of works
- [ ] Why every open source software is not free software?
  > [!info]- Ans
  > Some open source licenses are too restrictvie, so they so not qualify as free licenses.
- [ ] Show the use of `nice -n -20 ./a.out` in Linux OS.
  > [!info]- Ans
  > nice sets priority of a process when it starts
  > lower the nice value, higher the priority (-20 to 19).
  > a.out runs with highest priority
- [ ] Define a crontab to run a command at 8 PM on the 1st, 10th, and 20th of every month.
  > [!info]- Ans
  > 0 20 1,10,20 \* \*

---

- [ ] What is the expansion of CMS and ERP?
  > [!info]- Ans
  > content management system
  > Enterprise resource planning
- [ ] Define copy left license?
  > [!info]- Ans
  > downstream projects cannot add additional restrictions on the use of the software

### Part B

- [ ] Compare open source software with closed source software.
- [ ] Summarize the needs of open source software.
- [ ] Outline a shell script to get and set personality as `PER_BSD` using a system call.
- [ ] Illustrate ideal fair scheduling for the following process with 4ms CPU quanta time.
  > [!note]- Notes
  > 100/n %
  > | Process | Burst Time |
  > | ------- | ---------- |
  > | A | 8ms |
  > | B | 4ms |
  > | C | 16ms |
  > | D | 4ms |

---

- [ ] outline the structure of Linux OS
  > [!info]- Ans
  >
  > ###### layers
  >
  > - hw
  > - kernal
  > - shell
  > - user app

---

- [ ] process life cycle
  > [!info]- Ans
  > **program in execution**

### Part C

- [ ] Explain the basics syntax and examples of how to use the case statement in bash for pattern matching.

  > [!note]- Notes
  >
  > ```bash
  > #!/bin/bash
  > filename="document.txt"
  >
  > case $filename in
  >  *.txt)
  >    echo "This is a text file."
  >    ;;
  >  *.jpg|*.png)
  >    echo "This is an image file."
  >    ;;
  >  *)
  >    echo "Unknown file type."
  >    ;;
  > esac
  > ```

- [ ] Demonstrate the rules to be followed constructing a Red Black tree for the data 15, 10, 18, 14, 30, 25, 40, 60.
  > [!note]- Notes
  >
  > - every node - red || black
  > - root && leaf node == black
  > - every path from a node to its descendant leaves must have the same number of black nodes
  >
  > ###### rr conflict
  >
  > - uncle red
  >   - recolor dad and uncle
  >   - recolor grandpa if he is not root
  > - uncle black
  >   - rotation
  >   - recolor dad and grandpa

---

- [ ] Demonstrate the rules to be followed constructing a Red Black tree for the data 7, 15, 5, 13, 25
- [ ] explain user mode and kernel more process of the Linux operating system
