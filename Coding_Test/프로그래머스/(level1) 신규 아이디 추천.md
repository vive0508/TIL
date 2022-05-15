신규 아이디 추천 (level 1)
===

```python
def solution(new_id):
  answer = ''
  # 1단계
  new_id = new_id.lower()
  
  # 2단계
  for c in new_id:
    if c.isalpha() or c.isdigit() or c in "-_.":
      answer += c
      
  # 3단계
  while '..' in answer:
    answer = answer.replace('..', '.')
    
  # 4단계
  if answer and answer[0] == '.':
    answer = answer[1:]
  if answer and answer[-1] == '.':
    answer = answer[:-1]
    
  # 5단계
  if answer == '':
    answer = 'a'
  
  # 6단계
  answer = answer[:15]
  if answer[-1] == '.':
    answer = answer[:-1]
  print(answer)
  
  # 7단계
  while len(answer) < 3:
    answer += answer[-1]
    
  return answer
  
print(solution("...!@BaT#*..y.abcdefghijklm"))
```

[레퍼런스](https://coding-grandpa.tistory.com/93)
