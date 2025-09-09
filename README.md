# Hey there! 👋 I'm Hana

<div align="center">
  
[![Typing SVG](https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=500&size=24&pause=1000&color=6366F1&center=true&vCenter=true&width=600&lines=Frontend+Developer+%7C+AI+Enthusiast;Building+Smart+%26+Clean+Web+Apps;Always+Yearning%2C+Always+Building+%F0%9F%9A%80)](https://git.io/typing-svg)

</div>

---

## 🚀 **About Me**
I'm a **Frontend Developer** passionate about creating intelligent, user-centric applications. I transform ideas into interactive experiences using modern web technologies and AI integration.

```javascript
const hana = {
  location: "Sydney, Australia 🇦🇺",
  currentFocus: "Frontend Development + AI Integration",
  availableFor: "Frontend Developer Roles",
  learningGoal: "1% better every day",
  motto: "Building the future, one component at a time"
}
```

---

## 💼 **Currently Building**

### 🌸 **Spring Petals** - AI-Powered Floral Discovery Platform
```
🎯 Problem: Finding the perfect flowers for occasions is overwhelming
💡 Solution: AI agent that recommends flowers by meaning, creates vision boards, 
           provides care tips, and connects with local Sydney communities
🛠️ Tech: Next.js 14, OpenAI API, Supabase, Tailwind CSS, Geolocation API
📊 Impact: Helping users discover perfect florals for life's special moments
```
**[Live Demo](#) | [Code](#)**

### 🍰 **Crookie App** - AI-Enhanced Recipe Discovery
```
🎯 Problem: Finding recipes that match available ingredients and location
💡 Solution: Recipe app with AI-generated food images and Sydney location integration
🛠️ Tech: React, DALL-E API, Google Maps API, Firebase, PWA
📊 Impact: Personalized cooking experience for Sydney food lovers
```
**[Live Demo](#) | [Code](#)**

---

## 🛠️ **Tech Stack**

<div align="center">

### **Frontend Development**
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)

### **AI & Integration**
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?style=for-the-badge&logo=supabase&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)

### **Tools & Workflow**
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visual-studio-code&logoColor=white)
![Figma](https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white)

</div>

---

## 📊 **GitHub Analytics**

<div align="center">
  <img height="180em" src="https://github-readme-stats.vercel.app/api?username=yourusername&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true"/>
  <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=yourusername&layout=compact&langs_count=7&theme=tokyonight"/>
</div>

<div align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=yourusername&theme=tokyonight" alt="GitHub Streak" />
</div>

---

## 🏆 **What Sets Me Apart**

<table>
<tr>
<td valign="top" width="33%">

### 🎯 **Problem Solver**
- Identify real-world problems
- Design user-centric solutions  
- Implement with modern tech stack
- Iterate based on feedback

</td>
<td valign="top" width="33%">

### 🚀 **Fast Learner**
- Master new technologies like a sponge
- Apply learnings immediately
- Document and share knowledge
- Stay current with industry trends

</td>
<td valign="top" width="33%">

### 🤝 **Collaboration Ready**
- Clear communication skills
- Experience with modern workflows
- Open to feedback and mentorship
- Team player mindset

</td>
</tr>
</table>

---

## 💻 **Featured Code**

<details>
<summary>🤖 AI Integration Example</summary>

```typescript
// AI-powered flower recommendation system
export async function getFlowerRecommendations(occasion: string, mood: string) {
  const completion = await openai.chat.completions.create({
    model: "gpt-4-turbo-preview",
    messages: [{
      role: "system",
      content: "You are a floral expert who recommends flowers based on occasions and emotions."
    }, {
      role: "user", 
      content: `Recommend flowers for ${occasion} with a ${mood} mood. Include meaning and care tips.`
    }],
    temperature: 0.7,
  });
  
  return {
    recommendations: completion.choices[0].message.content,
    timestamp: new Date().toISOString()
  };
}
```

</details>

<details>
<summary>⚛️ React Component Example</summary>

```tsx
// Reusable project card component with TypeScript
interface ProjectCardProps {
  title: string;
  description: string;
  tech: string[];
  demoUrl: string;
  githubUrl: string;
  status: 'in-progress' | 'completed' | 'planning';
}

export const ProjectCard: React.FC<ProjectCardProps> = ({
  title, description, tech, demoUrl, githubUrl, status
}) => {
  return (
    <div className="bg-white rounded-lg p-6 shadow-md hover:shadow-lg transition-shadow">
      <h3 className="text-xl font-bold mb-2">{title}</h3>
      <p className="text-gray-600 mb-4">{description}</p>
      
      <div className="flex flex-wrap gap-2 mb-4">
        {tech.map(item => (
          <span key={item} className="bg-blue-100 text-blue-800 px-2 py-1 rounded text-sm">
            {item}
          </span>
        ))}
      </div>
      
      <div className="flex gap-3">
        <a href={demoUrl} className="bg-blue-600 text-white px-4 py-2 rounded hover:bg-blue-700">
          Live Demo
        </a>
        <a href={githubUrl} className="border border-gray-300 px-4 py-2 rounded hover:bg-gray-50">
          View Code
        </a>
      </div>
    </div>
  );
};
```

</details>

---



---

## 🌟 **Let's Connect & Collaborate**

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/hana-pham-601a551b0/)
[![Portfolio](https://img.shields.io/badge/Portfolio-Visit-FF5722?style=for-the-badge&logo=firefox&logoColor=white)](https://hanapham.com/)
[![Email](https://img.shields.io/badge/Email-Contact-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:the.hanapham@gmail.com)

</div>

### 💬 **Let's Chat About:**
- Frontend development opportunities in Sydney
- AI integration in web applications  
- React/Next.js best practices
- Career transitions into tech
- Collaboration on exciting projects

---

<div align="center">

### 🚀 **"Building the future, one component at a time"**

![Profile Views](https://komarev.com/ghpvc/?username=yourusername&color=6366f1&style=for-the-badge)

**⭐ If you find my projects interesting, consider giving them a star!**

</div>

---

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&height=100&section=footer" width="100%" />
</div>
