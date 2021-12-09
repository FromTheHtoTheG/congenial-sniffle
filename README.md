# congenial-sniffle
#GUI LOGIN FOR APP
#Dev by Hung Nguyen

from tkinter import *
from tkinter import font
def main_account_screen():
    main_screen = Tk()
#chon kich thuoc cho cua so
    main_screen.geometry("400x350")
#Chon tieu de cho cua so
    main_screen.title("Account Login cilent")


#Tao label
    Label(text="Choose Login Or Register", bg="blue", width="300", height="5", font=("Calibri",14)).pack()
    Label(text="").pack()

#Tao nut dang nhap
    Button(text="Login", height="2", width="30").pack()
    Label(text="").pack()

#Tao nut dang ki
    Button(text="Register", height="2", width="30").pack()
    
    main_screen.mainloop()
main_account_screen()


def register():
#widget hoat dong gan giong nhu la frame, nhun no hien thi tron cua so rieng biet, high level.
#nhu cac cua so thuong co cac thanh tieu de, vien va cac noi dung tren cua so khac.
#trong mainloop, chung ta phai vuot qua bien nhieu lan
    register_screen = Toplevel(main_sreen)
    register_screen.title("Register")
    register_screen.geometry("300x250")

#dat bien van ban
    username = StringVar()
    password = StringVar()
#Tao label huong dan dang ki/dang nhap
    Label(register_screen, text="Please enter details below", bg="blue").pack()
    Label(register_screen, text="").pack()
#Cai` Label cho nguoi` dung
    username_label = Label(register_screen, text="Username * ")
    username_label.pack()

#Cai ten dang nhap vao
#Entry se la standard Tkinter widget used to enter
    username_entry = Entry(register_screen, textvariable= username)
    username_entry.pack()
#set password label
    password_label = Label(register_screen, text="Password * ")
    password_label.pack()
#set password entry
    password_entry = Entry(register_screen, textvariable= password)

    Label(register_screen, text= "").pack() 

#set register button
    Button(register_screen, text="Register", width= 10, height= 1, bg="blue").pack()
    global 
    Button(text="register", height="2", width="30", command=register).pack()
