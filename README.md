# latihan-1-pratikum-8
    try:
        num1 = float(input("Masukkan angka pertama: "))
        operator = input("Masukkan operator (+, -, *, /): ")
        num2 = float(input("Masukkan angka kedua: "))
    
        if operator == '+':
            result = num1 + num2
        elif operator == '-':
            result = num1 - num2
        elif operator == '*':
            result = num1 * num2
        elif operator == '/':
            if num2 == 0:
                raise ZeroDivisionError
            result = num1 / num2
        else:
            raise Exception("Operator tidak valid")
    
        print(f"Hasil: {result}")

    except ValueError:
        print("Error: Masukkan angka yang valid.")
    except ZeroDivisionError:
        print("Error: Pembagian dengan nol tidak diperbolehkan.")
    except Exception as e:
        print(f"Error: {e}")

  # Menghasilkan seperti ini
  <img width="361" height="97" alt="image" src="https://github.com/user-attachments/assets/100441a9-8ded-41a2-990a-ae888c530d96" />

  # latihan 2 pratikum 8
      nilai = [80, 90, 'A', 70, 100, 'B']
    total_nilai = 0
    jumlah_valid = 0

    for item in nilai:
        try:
            total_nilai += item
            jumlah_valid += 1
        except TypeError:
            # Melewati item yang bukan angka
            pass

    if jumlah_valid > 0:
        rata_rata = total_nilai / jumlah_valid
    else:
        rata_rata = 0

    print(f"Rata-rata dari data yang valid adalah: {rata_rata}")

# Menghasilkan seperti ini
<img width="367" height="98" alt="image" src="https://github.com/user-attachments/assets/4012afd3-aea5-4680-9e41-ffd3fae774cf" />

