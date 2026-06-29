class longestWindow:
    def lengthOfWindow(self,s):
        char_set=set()
        left=0
        max_len=0
        for right in range(len(s)):
            current=s[right]
            while current in char_set:
                char_set.remove(s[left])
                left+=1
            char_set.add(current)
            max_len=max(max_len,right-left+1)
        return max_len
#MAIN
l=longestWindow()
print(l.lengthOfWindow("abcabcbb"))