# Python-Project</br>
print("Title of program: Encouragement bot")</br>
print()</br>
while True:</br>
  description = input("Use one word to describe how you are feeling right now.")</br>
</br>
  list_of_words = description.split()</br>
</br>
  feelings_list = []</br>
  encouragement_list = []</br>
  counter = 0</br>
  </br>
  for each_word in list_of_words:</br>
    </br>
    if each_word == "sad":</br>
      feelings_list.append("sad")</br>
      encouragement_list.append("tomorrow will be a better day")</br>
      counter += 1</br>
    if each_word == "happy":</br>
      feelings_list.append("happy")</br>
      encouragement_list.append("to keep smiling")</br>
      counter += 1</br>
    if each_word == "tired":</br>
      feelings_list.append("tired")</br>
      encouragement_list.append("you are stronger than you think")</br>
      counter += 1</br>
    if each_word == "annoyed":</br>
      feelings_list.append("annoyed")</br>
      encouragement_list.append("to calm down and take a step back")</br>
      counter += 1</br>
    if each_word == "energetic":</br>
      feelings_list.append("energetic")</br>
      encouragement_list.append("to be energetic the way you are")</br>
      counter += 1</br>
</br>
  if counter == 0:</br>
    
      output = "Sorry I don't really understand. Please use only one word to describe how you are feeling currently."</br>
</br>
  elif counter == 1:</br>
    
      output = "It seems that you are feeling quite " + feelings_list[0] + ". Always remember that "+ encouragement_list[0] + "! Hope you feel better :)"  </br>
</br>
  else:</br>
</br>
    feelings = ""    </br>
    for i in range(len(feelings_list)-1):</br>
      feelings += feelings_list[i] + ", "</br>
    feelings += "and " + feelings_list[-1]</br>
    </br>
    encouragement = ""    </br>
    for j in range(len(encouragement_list)-1):</br>
      encouragement += encouragement_list[i] + ", "</br>
    encouragement += "and " + encouragement_list[-1]</br>
</br>
    output = "It seems that you are feeling quite " + feelings + ". Always remember "+ encouragement + "! Hope you feel better :)"</br>
</br>
  print()</br>
  print(output)</br>
  print()</br>
