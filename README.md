# Warsztat
## Repozytorium stworzone w ramach ćwiczeń z przedmiotu _"Warsztat Badacza Danych"_

**Omawiane zagadnienia:**
1. Linux
   * podstawowe polecenia
   * uprawnienia
   * ...
2. Markdown
   * formatowanie tekstu
   * linki
   * cytowanie
   * ...
3. Git
   * zakładanie konta GitHub
   * tworzenie repozytorium
   * ...
   
[Link do strony z materiałami z przedmiotu](https://drive.google.com/drive/folders/1Z5ljIlwnrMjgBnk_0bnEF7_Yp0OjJ0TI)  
[Link do strony UWM][UWM]

![Logo MIR](https://mir.gdynia.pl/wp-content/uploads/2016/04/logo_2017-AG.png)

[UWM]: http://www.uwm.edu.pl/
```python
def read_data(self, data_file_path, header=False):
  try:
      with open(data_file_path, "r") as file_reader:
          line_no = 1
          for line in file_reader:
              line_split = line.replace("\n", "").split(sep=",")
              if header & line_no == 1:
                  self.labels = line_split
              else:
                  self.dataset.append(line_split)
              line_no = line_no + 1
  except IOError:
      print("Exception: IOError")
```
