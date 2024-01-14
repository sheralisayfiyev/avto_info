# avto_info
sodda funksiyalar ustida amallar

def avto_info(kompaniya, model, rangi, karobka, yili, narxi=None):
    avto = {"kompaniya":kompaniya,
            "model":model,
            "Rang":rangi,
            "karobka":karobka,
            "yil":yili,
            "narh":narxi}
    return avto
def avto_kirit():
    print("Saytimizdagi avtolar ro'yxatini shaklantiramiz")
    avtolar = []
    while True:
        print("Quyidagi malumotlarni tuldiring")
        kompaniya=input("kompaniya: ")
        model=input("Modeli: ")
        rangi=input("Rangi: ")
        karobka=input("Karobka: ")
        yili=input("Yili: ")
        narxi=input("Narxi: ")
        avtolar.append(avto_info(kompaniya,model,rangi,karobka,yili,narxi))
        javob=input("Yana avto qushasizmi? (yes/no): ")
        if javob=="no":
            break
def avto_print():
    """Avtomobillar haqida malumotlar"""
    print(f"{avto_info['rang'].title()} {avto['kompaniya'].upper()} "
          f"{avto_info['model'].upper()}, {avto_info['karobka']} karobka, "
          f"{avto_info['yil']}-yil, {avto_info['narx']}$")
