  data = input('숫자로 이루어진 문자열을 입력하세요. ')
  length = len(data)

  mul = 0
  sum = 0

  for i in range(0, length):
      if int(data[i]) != 0:
          mul = mul * int(data[i])
      elif int(data[i]) == 0 and mul > 1:
          sum = sum + mul
          mul = 1
      else:
          mul = 1
  result = sum + mul
  print(result)   
