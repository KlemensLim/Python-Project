# Python-Project
print("Title of program: Encouragement bot")
print()
while True:
  description = input("Hi there! Could you use one word to describe how you are feeling right now?")

  list_of_words = description.split()

  feelings_list = []
  encouragement_list = []
  counter = 0

  for each_word in list_of_words:

    if each_word == "sad":
      feelings_list.append("sad")
      encouragement_list.append("tomorrow will be a better day")
      counter += 1
    if each_word == "happy":
      feelings_list.append("happy")
      encouragement_list.append("to keep smiling")
      counter += 1
    if each_word == "tired":
      feelings_list.append("tired")
      encouragement_list.append("you are stronger than you think")
      counter += 1
    if each_word == "annoyed":
      feelings_list.append("annoyed")
      encouragement_list.append("to calm down and take a step back")
      counter += 1
    if each_word == "energetic":
      feelings_list.append("energetic")
      encouragement_list.append("to be energetic the way you are")
      counter += 1

  if counter == 0:
    
      output = "Sorry I don't really understand. Please use only one word to describe how you are feeling currently."

  elif counter == 1:
    
      output = "It seems that you are feeling quite " + feelings_list[0] + ". Always remember that "+ encouragement_list[0] + "! Hope you feel better :)"  

  else:
  
    feelings = ""    
    for i in range(len(feelings_list)-1):
      feelings += feelings_list[i] + ", "
    feelings += "and " + feelings_list[-1]
    
    encouragement = ""    
    for j in range(len(encouragement_list)-1):
      encouragement += encouragement_list[i] + ", "
    encouragement += "and " + encouragement_list[-1]
    
    output = "It seems that you are feeling quite " + feelings + ". Always remember "+ encouragement + "! Hope you feel better :) Bye!!!"

  print()
  print(output)
  print()
