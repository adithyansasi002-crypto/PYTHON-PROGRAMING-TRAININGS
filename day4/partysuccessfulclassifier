day=input().strip()  #strip-remove leading and trailing function
attendees=int(input())
def PartySuccessfulClassifier(day,attendees):
    weekdays=['MON','TUE','WED','THUR']
    weekends=['FRI','SAT','SUN']
    if day not in weekdays and day not in weekends:
        return 'INVALID DAY'
    if attendees<0:
        return 'INVALID ATTENDEES'
    if day in weekdays:
        if 700<=attendees<=1000:
            return 'Successfull'
        else:
            return "Unsuccessfull"
    if day in weekends:
        if attendees>=1500:
            return 'Successfull'
        else:
            return "Unsuccessfull"
a=PartySuccessfulClassifier(day,attendees)
print(a)