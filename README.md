# LeetCode-557.-Reverse-Words-in-a-String-III

class Solution:
    def reverseWords(self, s: str) -> str:
        word_list = s.split(' ')
        # print(word_list)
        result = ""
        
        for i in range(len(word_list)):
            if i != len(word_list) - 1:
                result += word_list[i][::-1] + ' '
            else:
                result += word_list[i][::-1]
                
        return result
