#Min&Jun's Cafe - serving Game

import tkinter as tk
import tkinter.messagebox
import time

customer1 = """
            ----------
            |        |
            |        |
            |        |
            | ^   ^  |
        0---|   U    |---0
            |        |
            |        |
            |        |
            |        |
            |        |
            ----------

"""

customer2 = """
            ----------
            |        |
            |        |
            |        |
            | -   -  |
        0---|   ^    |---0
            |        |
            |        |
            |        |
            |        |
            |        |
            ----------

"""

customer3 = """
            ----------
            |        |
            |        |
            |        |
            | 0   ^  |
        0---|   v    |---0
            |        |
            |        |
            |        |
            |        |
            |        |
            ----------

"""

customer4 = """
            ----------
            |        |
            |        |
            |        |
            | 0   0  |
        0---|   <    |---0
            |        |
            |        |
            |        |
            |        |
            |        |
            ----------

"""


customer5 = """
            ----------
            |        |
            |        |
            |        |
            | 0   <  |
        0---|   U    |---0
            |        |
            |        |
            |        |
            |        |
            |        |
            ----------

"""

customer6 = """
            ----------
            |        |
            |        |
            |        |
            | T   T  |
        0---|   ^    |---0
            |        |
            |        |
            |        |
            |        |
            |        |
            ----------

"""

customer7 = """
            ----------
            |        |
            |        |
            |        |
            | U   U  |
        0---|   ~    |---0
            |        |
            |        |
            |        |
            |        |
            |        |
            ----------

"""

customer8 = """
            ----------
            |        |
            |        |
            |        |
            | U   0  |
        0---|   <    |---0
            |        |
            |        |
            |        |
            |        |
            |        |
            ----------

"""

customer9 = """
            ----------
            |        |
            |        |
            |        |
            | 0   0  |
        0---|   0    |---0
            |        |
            |        |
            |        |
            |        |
            |        |
            ----------

"""

customer10 = """
            ----------
            |        |
            |        |
            |        |
            | X   X  |
        0---|   ~    |---0
            |        |
            |        |
            |        |
            |        |
            |        |
            ----------
"""

vanilla_IC = """
                  ^
               (    )
            ------------
           (            )
        -------------------
       (                   )
        -------------------
       |                   |
       |                   |
       |      Vanilla      |
       |     Ice Cream     |
       |                   |
       |                   |
       |                   |
       ---------------------
        

"""
level = 0

def korea_click():
    btn1["text"] = "메뉴"
    btn2["text"] = "게임 시작"
    btn3["text"] = "게임 방법"
    btn4["text"] = "손님 정보"
    btn5["text"] = "상점"
    btn6["text"] = "손님 부르기"
    btn7["text"] = "언어 - 한국어"
    btn8["text"] = "언어 - 영어"

def eng_click():
    btn1["text"] = "Menu"
    btn2["text"] = "Game Start"
    btn3["text"] = "Tutorial"
    btn4["text"] = "Customers Info"
    btn5["text"] = "Store"
    btn6["text"] = "Call Customers"
    btn7["text"] = "Lauguage - Korean"
    btn8["text"] = "Lauguage - English"

def game_start():
    print("========== Game Start! ==========")
    print("                                 ")
    print("카페 도우미 : 안녕하세요? 저는 당신의 첫 카페 개장을 도울 <카페 도우미> 예요!", time.time())
    time.sleep(1.8)
    print("카페 도우미 : 먼저 상점에서 <나무 테이블> 을 구매해봅시다.")

def store_click():
    win2 = tk.Tk()
    win2.title("상점")
    btn_01 = tk.Button(win2, text="나무 테이블", command=tree_table)
    btn_01.pack()
    btn_02 = tk.Button(win2, text="나무 의자", command=tree_chair)
    btn_02.pack()
    btn_03 = tk.Button(win2, text="티 머신", command=tea_machine)
    btn_03.pack()
    btn_04 = tk.Button(win2, text="바닐라 아이스크림 냉동고", command=vanilla_Icream)

def tree_table():
    msg1 = tk.messagebox.showinfo("완료 메시지", "<나무 테이블> 이 구매 완료되었습니다.")
    print("카페 도우미 : 나무 테이블이 있으니 이젠 <나무 의자>도 있어야하겠죠? 상점에 가서 <나무 의자> 를 구매해보세요!")

def tree_chair():
    msg2 = tk.messagebox.showinfo("완료 메시지", "<나무 의자> 가 구매 완료되었습니다.")
    print("카페 도우미 : 마지막으로 <티 머신> 도  구매해보세요.")

def tea_machine():
    msg3 = tk.messagebox.showinfo("완료 메시지", "<티 머신> 이 구매 완료되었습니다.")
    print("카페 도우미 : 잘 하셨어요! 이제 손님 부르기 버튼을 클릭하여 손님을 불러보세요!")

def call_cust():
    print("손님 부르는 중", time.time())
    time.sleep(0.6)
    print("손님 부르는 중 .", time.time())
    time.sleep(0.6)
    print("손님 부르는 중 . .", time.time())
    time.sleep(0.6)
    print("손님 부르는 중 . . .", time.time())
    time.sleep(0.6)
    print("완료!", time.time())
    time.sleep(3)
    print(customer1, time.time())
    time.sleep(2)
    print("손님 1 : 안녕하세요! 첫 카페 개장 축하드려요~", time.time())
    time.sleep(3)
    print("손님 1 : 아, 제 이름은 '루니아 제시' 예요! 사람들은 모두 저를 '루시'라고 불러요. 여민 님도 편하신대로 불러주세요!", time.time())
    time.sleep(6)
    print("그런데 <바닐라 아이스크림> 메뉴가 있나요? 이 근처에 파는곳이 없어서 못 먹었거든요. 준비해주신다면 제가 작은 선물을 드릴게요!", time.time())
    time.sleep(8)
    print("카페 도우미 : 루시 손님이 바닐라 아이스크림 메뉴를 기다리고 있어요! 어서 상점에서 <바닐라 아이스크림 냉동고>를 구입하세요.")

def vanilla_Icream():
    msg4 = tk.messagebox.showinfo("확인 메시지", "<바닐라 아이스크림 냉동고>가 구매 완료되었습니다.")
    print("카페 도우미 : 잘 하셨어요! 이제 메뉴 버튼에서 <바닐라 아이스크림>을 클릭해보세요.")

def menu_click():
    win3 = tk.Tk()
    win3.title("메뉴")
    menu_01 = tk.Button(win3, text="티")
    menu_01.pack()
    menu_02 = tk.Button(win3, text="바닐라 아이스크림", command=vanillaIC_serving)
    menu_02.pack()

def vanillaIC_serving():
    print(vanilla_IC)
    print("카페 도우미 : 그 다음 손님 정보 버튼을 클릭해 서빙 버튼을 클릭하세요.")


def cust_info():
    win4 = tk.Tk()
    win4.title("Customers Info")
    c_info1 = tk.Label(win4, text="손님 1 : 루시")
    c_info2 = tk.Label(win4, text=customer1)
    c_btn1 = tk.Button(win4, text="서빙하기", command=serving_click)
    c_info1.pack()
    c_info2.pack()
    c_btn1.pack()

def serving_click():
    def vanillaC_serving():
        msg5 = tk.messagebox.showinfo("확인 메시지", "루시 손님에게 <바닐라 아이스크림> 메뉴를 서빙했습니다.")
        print(customer1)
        print("정말 감사해요! 선물은 레벨업이랍니다! 아이스크림 잘 먹었어요~")
        level=1
        msg6 = tk.messagebox.showinfo("레벨업 메시지", f"축하합니다! 레벨{level}로 레벨업하였습니다!")


win = tk.Tk()
win.title("Min&Jun's Cafe - serving Game")


#Buttons
btn1 = tk.Button(win, text="Menu", command=menu_click)
btn1.pack()
btn2 = tk.Button(win, text="Game Start", command=game_start)
btn2.pack()

btn3 = tk.Button(win, text="Tutorial")
btn3.pack()

btn4 = tk.Button(win, text="Customers Info", command=cust_info)
btn4.pack()

btn5 = tk.Button(win, text="Store", command=store_click)
btn5.pack()

btn6 = tk.Button(win, text="Call Customers", command=call_cust)
btn6.pack()

btn7 = tk.Button(win, text="Lauguage - Korean", command=korea_click)
btn7.pack()

btn8 = tk.Button(win, text="Lauguage - English", command=eng_click)
btn8.pack()





win.mainloop()
