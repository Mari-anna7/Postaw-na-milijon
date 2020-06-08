# Postaw-na-milijon
# Projket z programowanka - dodatkowy termin

from tkinter import *
import tkinter as tk

glowne_okno = tk.Tk()
glowne_okno.title("Postaw na miljon")
glowne_okno.geometry("900x650")

##########################
zapadnia1 = tk.Label(glowne_okno, bg = "#80c1ff", bd=10)
zapadnia1.place(relx=0.20, rely=0.25, relwidth=0.15, relheight=0.35, anchor='n')

button1 = tk.Button(zapadnia1, text = "+", font=50)
button1.place(relx=0.35, rely=0.7, relwidth=0.3, relheight=0.2, anchor='n')
button2 = tk.Button(zapadnia1, text = "-", font=50)
button2.place(relx=0.65, rely=0.7, relwidth=0.3, relheight=0.2, anchor='n')

odpowiedz1 = tk.Label(zapadnia1, text = "A", font=50,  bg = "#80c1ff")
odpowiedz1.place(relx=0.5, rely=0, relwidth=0.3, relheight=0.2, anchor='n')

##########################

zapadnia2 = tk.Label(glowne_okno, bg = "#80c1ff", bd=10)
zapadnia2.place(relx=0.40, rely=0.25, relwidth=0.15, relheight=0.35, anchor='n')

button3 = tk.Button(zapadnia2, text = "+", font=50)
button3.place(relx=0.35, rely=0.7, relwidth=0.3, relheight=0.2, anchor='n')
button4 = tk.Button(zapadnia2, text = "-", font=50)
button4.place(relx=0.65, rely=0.7, relwidth=0.3, relheight=0.2, anchor='n')

odpowiedz2 = tk.Label(zapadnia2, text = "B", font=50,  bg = "#80c1ff")
odpowiedz2.place(relx=0.5, rely=0, relwidth=0.3, relheight=0.2, anchor='n')

##########################

zapadnia3 = tk.Label(glowne_okno, bg = "#80c1ff", bd=10)
zapadnia3.place(relx=0.60, rely=0.25, relwidth=0.15, relheight=0.35, anchor='n')

button5 = tk.Button(zapadnia3, text = "+", font=50)
button5.place(relx=0.35, rely=0.7, relwidth=0.3, relheight=0.2, anchor='n')
button6 = tk.Button(zapadnia3, text = "-", font=50)
button6.place(relx=0.65, rely=0.7, relwidth=0.3, relheight=0.2, anchor='n')

odpowiedz3 = tk.Label(zapadnia3, text = "C", font=50,  bg = "#80c1ff")
odpowiedz3.place(relx=0.5, rely=0, relwidth=0.3, relheight=0.2, anchor='n')

##########################

zapadnia4 = tk.Label(glowne_okno, bg = "#80c1ff", bd=10)
zapadnia4.place(relx=0.80, rely=0.25, relwidth=0.15, relheight=0.35, anchor='n')

button7 = tk.Button(zapadnia4, text = "+", font=50)
button7.place(relx=0.35, rely=0.7, relwidth=0.3, relheight=0.2, anchor='n')
button8 = tk.Button(zapadnia4, text = "-", font=50)
button8.place(relx=0.65, rely=0.7, relwidth=0.3, relheight=0.2, anchor='n')

odpowiedz4 = tk.Label(zapadnia4, text = "D", font=50,  bg = "#80c1ff")
odpowiedz4.place(relx=0.5, rely=0, relwidth=0.3, relheight=0.2, anchor='n')

def gra():
    kasa_gracza = 1000000
    for i in range(4):
        if kasa_gracza == 0:
            break
        zapadnia_1 = 0
        zapadnia_2 = 0
        zapadnia_3 = 0
        zapadnia_4 = 0
        kasa_gracza = zapadnia_1
    for i in range(3):
        if kasa_gracza == 0:
            break
        zapadnia_1 = 0
        zapadnia_2 = 0
        zapadnia_3 = 0
        zapadnia_4 = 0
        kasa_gracza = zapadnia_1
    if kasa_gracza == 0:
        zapadnia_1 = 0
        zapadnia_2 = 0
        kasa_gracza = zapadnia_1
    if kasa_gracza > 0:
        print("Gratuluję wygrałeś")

glowne_okno.mainloop()
