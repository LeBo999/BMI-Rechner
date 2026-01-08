def bmi_kategorie(bmi):
   if bmi < 18.5:
      return "Untergewicht"

   elif bmi < 25:
      return "Normalgewicht"

   elif bmi < 30:
     return "Übergewicht"

   elif bmi > 30:
     return "Adipositas"

groesse = int(input("Wie groß bist du (in cm) "))
gewicht = int(input("Wie schwer bist du (in kg) "))

bmi = gewicht / (groesse / 100) ** 2
print("Dein BMI ist: ", bmi)
print("Du hast", bmi_kategorie(bmi))
