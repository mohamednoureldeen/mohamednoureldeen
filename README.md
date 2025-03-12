```typescript
type TechStack = 
  | "Angular"
  | "TypeScript"
  | "JavaScript"
  | "HTML & CSS"
  | "SASS"
  | "Tailwind CSS"
  | "Bootstrap"
  | "Frontend Architecture";

interface DeveloperProfile {
  fullName: string;
  title: string;
  skills: TechStack[];
  bio: string;
  getIntroduction: () => string;
}

const myProfile: DeveloperProfile = {
  fullName: "Mohamed Noureldeen",
  title: "Frontend Developer",
  skills: [
    "Angular",
    "TypeScript",
    "JavaScript",
    "HTML & CSS",
    "SASS",
    "Tailwind CSS",
    "Bootstrap",
    "Frontend Architecture",
  ],
  bio: "Passionate about building modern, scalable, and visually appealing web applications.
 I specialize in crafting elegant UI components with Angular and optimizing user experiences with SASS,
 Tailwind CSS, and Bootstrap.",
  getIntroduction() {
    return `👋 Hey there! I'm ${this.fullName}, a ${this.title}. My expertise includes ${this.skills.join(
      ", "
    )}. ${this.bio}`;
  },
};
console.log(myProfile.getIntroduction());
```
