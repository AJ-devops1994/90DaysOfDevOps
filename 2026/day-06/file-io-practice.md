
touch notes.txt`
echo "Line 1" > notes.txt
echo "Line 2" >> notes.txt
echo "Line 3" | tee -a notes.txt
cat notes.txt
head -n 2 notes.txt
tail -n 2 notes.txt


Hand-on practice:
361  touch notes.txt
  362  echo "Hey, I am in a90daysofdevops journey\n brushing up my linux concepts\n learning new things > notes.txt
  363  echo "Hey, I am in a90daysofdevops journey\n brushing up my linux concepts\n learning new things" > notes.txt
  364  cat notes.txt
  365  echo "Hey, I am in a90daysofdevops journey\nbrushing up my linux concepts\nlearning new things" > notes.txt
  366  cat notes.txt
  367  echo -e "Hey, I am in a90daysofdevops journey\nbrushing up my linux concepts\nlearning new things" > notes.txt
  368  cat notes.txt
  369  echo -e "this is my day6 of 90daysofdevops\nfocusing more on hands-on\nThank you" >>notes.txt
  370  cat notes.txt
  371  echo "\nhey friend I want you to practice with me, lets grow together" | tee -a notes.txt
  372  cat notes.txt
  373  echo -e "\nhey friend I want you to practice with me, lets grow together" | tee -a notes.txt
  374  cat notes.txt
  375  head -n 3 notes.txt
  376  tail -n 2 notes.txt
  377  history


