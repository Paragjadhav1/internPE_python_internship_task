# internPE_python_internship_task
TASK 1

"""Task 1:
Task : Make a Digital Clock With the help of Python After that make a separate Video on it and post On LinkedIn.And Tag Internpe
This Below Video is for your reference only.
You can show your skills style in your own way DeadLine is End of this week"""

import tkinter as tk
import time

def update_clock():
    current_time = time.strftime('%H:%M:%S')
    label.config(text=current_time)
    label.after(1000, update_clock)

root = tk.Tk()
root.title("Digital Clock")

label = tk.Label(root, font=('calibri', 40, 'bold'), background='black', foreground='white')
label.pack(anchor='center')

update_clock()

root.mainloop()

