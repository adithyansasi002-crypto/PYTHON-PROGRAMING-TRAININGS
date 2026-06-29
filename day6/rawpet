#inheritance
class VISACARD:
    def __init__(self,holder_name,card_number):
        self.holder_name=holder_name
        self.card_number=card_number
    def display_details(self):
        print(self.holder_name)
        print(self.card_number)
    def compute_rewards(self,amt):
        rew=amt*0.01
        print("The reward for VISACARD is:",rew)
class HPVISACARD(VISACARD):
    def compute_rewards(self,purchase_type, amt): # fn is same but different classes-->polymorphism 
        rew=amt*0.01
        if purchase_type=='Fuel':
            rew=rew+10
        print("The reward for HPViSACARD is:",rew)
#input
card_type=input("VISA/HPVISA ").strip()
if card_type not in ['VISA','HPVISA']:
    print("INVALID CHOICE")
else:
    holder_name=input("Name: ").strip()
    card_number=input('Card Number: ').strip()
    amt=float(input("Amount:"))
    purchase_type=input("Purchase Type: ")
    #instances
    if card_type=='VISA':
        card=VISACARD(holder_name,card_number)
        card.display_details()
        card.compute_rewards(amt)
    else:
        card=HPVISACARD(holder_name,card_number)
        card.display_details()
        card.compute_rewards(purchase_type,amt)