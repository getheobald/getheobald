<!--
- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->

```
class Profile {
  public String name;
  public String[] pronouns;
  public String school;
  public String year;
  public String major;
  private double GPA;
  public String sport;
  public String[] hobbies;

  public Profile() {
    this.name = "Grace Theobald";
    this.pronouns = {"She", "Her"};
    this.school = "Northeastern University";
    this.year = "Junior";
    this.major = "Computer Science and Behavioral Neuroscience";
    this.GPA = 3.89;
    this.sport = "NCAA D1 Rowing";
    this.hobbies = {"Mountaineering", "Skiing", "Backpacking", "Guitar", "Audiobooks"};
  }

  public static void main(String[] args) {
    Profile getheobald = new Profile();
    getheobald.printProfile();
    getheobald.printActivitiesAndHobbies();
  }

  public void printProfile() {
    System.out.println("Hi, my name is " + this.name + "! My pronouns are " + this.pronouns + ". I'm a " + this.class +
                      " at " + this.school + " studying " + this.major + " with a GPA of " + this.GPA + ".");
  }

  public void printActivitiesAndHobbies() {
    StringBuilder hobbiesString = new StringBuilder();
    for (int i = 0; i < this.hobbies.length; i++) {
      hobbiesString.append(this.hobbies[i]);
      if (i < this.hobbies.length - 1) {
        hobbiesString.append(", ");
      }
    }
    System.out.println("I do " + this.sport + " and my favorite hobbies are " + hobbiesString + ".");
  }
}
```
