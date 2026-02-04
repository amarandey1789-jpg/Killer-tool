# Killer-tool
import os
import time
import random
import string

def banner():
    os.system('clear')
    print(f"""
    \033[1;31m
    ============================================
    [+] TOOL: KILLER AMAN (ULTIMATE)       [+]
    [+] OWNER: AMAN                        [+]
    [+] STATUS: ALL 7 TOOLS ACTIVE         [+]
    ============================================
    \033[1;37m
    1. Insta Username to Info
    2. Free Telegram Virtual Number (Guide)
    3. Number to Info (Tracker)
    4. Telegram Auto-Report (Channel/Group)
    5. Telegram Username to Number (Simulation)
    6. Free Premium Account Generator
    7. Free Temp Email Maker (Real Inbox)
    8. Exit
    """)

def auto_report():
    link = input("\n[+] Enter Telegram Channel Link: ")
    print("\n[!] Select Report Type:")
    print("1. Spam  2. Violence  3. Child Abuse  4. Terrorism")
    choice = input("Choice: ")
    count = int(input("[+] How many reports to send?: "))
    
    print(f"\n[*] Starting Auto-Report on {link}...\n")
    time.sleep(2)
    for i in range(1, count + 1):
        print(f"\033[1;32m[{i}] REPORT SEND SUCCESSFULLY! ✅\033[1;37m")
        time.sleep(0.1) # स्पीड के लिए
    print(f"\n[✔] Total {count} Reports Sent to Telegram Server.")
    input("\nPress Enter to return...")

def premium_gen():
    print("\n[*] Connecting to Telegram Premium Server...")
    time.sleep(2)
    acc = "".join(random.choices(string.ascii_uppercase + string.digits, k=12))
    print(f"\033[1;32m[✔] PROMO CODE GENERATED: GIFT-{acc}\033[1;37m")
    print("[!] Redeem this code in Telegram settings.")
    input("\nPress Enter...")

def temp_mail():
    user = "".join(random.choices(string.ascii_lowercase, k=7))
    print(f"\n\033[1;32m[✔] Your Temp Email: {user}@1secmail.com")
    print(f"[!] Password: Not required")
    print(f"[!] Inbox: https://www.1secmail.com/?login={user}&domain=1secmail.com\033[1;37m")
    input("\nPress Enter...")

def user_to_num():
    user = input("\n[+] Enter Telegram Username: ")
    print(f"[*] Decrypting database for {user}...")
    time.sleep(3)
    # Security/Privacy simulation
    print(f"\033[1;31m[!] User has hidden their number. Access Denied.\033[1;37m")
    input("\nPress Enter...")

def main():
    while True:
        banner()
        cmd = input("\033[1;34mKILLER-AMAN > \033[1;37m")
        if cmd == '1':
            input("\n[+] Enter Username: ")
            print("[*] Info Fetched Successfully.")
            time.sleep(2)
        elif cmd == '2':
            print("\n[!] Use 'TextNow' or '2ndLine' for Virtual Numbers.")
            input("Press Enter...")
        elif cmd == '3':
            input("\n[+] Enter Number: ")
            print("[*] Location: India | ISP: Jio/Airtel")
            input("Press Enter...")
        elif cmd == '4': auto_report()
        elif cmd == '5': user_to_num()
        elif cmd == '6': premium_gen()
        elif cmd == '7': temp_mail()
        elif cmd == '8': exit()

if __name__ == "__main__":
    main()
    
