public class main {
    public main() {
    }

    public static void main(String[] args) {
        Sotrudnik[] sotrudniks = new Sotrudnik[]{new Sotrudnik("Иванов", "Иван", "Директор", "Ivan@director.ru", "85557551425", 50000, 25), 
        new Sotrudnik("Петров", "Денис", "Менеджер", "petrov@ya.ru", "72558775525", 40000, 30), new Sotrudnik("Агутин", "Леонид", "Водитель", "agutin@ya.ru", "72558775526", 35000, 40), new Sotrudnik("Сидоров", "Никита", "дворник", "sidorov@ya.ru", "72558775528", 30000, 55), new Sotrudnik("Романова", "Анастасия", "Секретарь", "romanova@ya.ru", "72558775527", 30000, 20)};
        int minAge = 40;
        Sotrudnik[] var3 = sotrudniks;
        int var4 = sotrudniks.length;

        for(int var5 = 0; var5 < var4; ++var5) {
            Sotrudnik sotrudnik = var3[var5];
            if (sotrudnik.age > minAge) {
                sotrudnik.printInfo();
                System.out.println();
            }
        }

    }
}
public class Sotrudnik {
    String surname;
    String name;
    String post;
    String email;
    String phone;
    int salary;
    int age;

    Sotrudnik(String surname, String name, String post, String email, String phone, int salary, int age) {
        this.surname = surname;
        this.name = name;
        this.post = post;
        this.email = email;
        this.phone = phone;
        this.salary = salary;
        this.age = age;
    }

    void printInfo() {
        System.out.println("Фамилия:" + this.surname);
        System.out.println("Имя:" + this.name);
        System.out.println("Должность:" + this.post);
        System.out.println("Email:" + this.email);
        System.out.println("Телефон:" + this.phone);
        System.out.println("Зарплата:" + this.salary);
        System.out.println("Возраст:" + this.age);
    }
}
