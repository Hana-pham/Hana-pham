# Hey there! 👋 I'm Hana

<div align="center">
  
[![Typing SVG](https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=500&size=24&pause=1000&color=FF69B4&center=true&vCenter=true&width=600&lines=Frontend+Developer+%7C+AI+Engineer;Building+Smart+%26+Beautiful+Web+Apps;React+%7C+Next.js+%7C+TypeScript+%7C+Node.js)](https://git.io/typing-svg)

</div>

## 🚀 About Me

I'm a **Frontend Developer** passionate about creating intelligent, user-centric applications. I combine modern web technologies with AI to solve real-world problems.

```javascript
const hana = {
  location: "Sydney, Australia 🇦🇺",
  currentFocus: "Full-Stack Development + AI Integration",
  availableFor: "Frontend & Software Engineering Roles",
  learning: ["System Design", "React Native", "Machine Learning"],
  motto: "Building technology that makes a difference"
}
```

---

## 🚀 Featured Projects

| Project | Tech Stack | Description |
|---------|------------|-------------|
| **[Luna](https://luna-demo.vercel.app)** - Women's Wellness Platform | `React Native` `TypeScript` `Node.js` `PostgreSQL` `OpenAI API` `TensorFlow` `JWT` | AI-powered wellness platform with cycle-aware nutrition tracking and eating disorder prevention protocols |
| **[SpringPetals](https://springpetals.vercel.app)** - AI Floral Discovery | `Next.js 14` `TypeScript` `Supabase` `GPT-4` `DALL-E 3` `Mapbox GL` | AI-driven flower recommendations with local Sydney florist integration and care guides |
| **[Zippy](#)** - Design-to-Code Converter | `Python` `TypeScript` `GPT-4 Vision` `Figma API` `Node.js` | Automated tool reducing design-to-code time by 70% with 80% accuracy |
| **[Movie Library](#)** - Native Mobile Apps | `Swift` `Kotlin` `UIKit` `Jetpack Compose` `GraphQL` `Redis` | Cross-platform movie browsing with real-time booking and offline support |

---

## 🛠️ Technical Skills

<div align="center">

### Languages & Frameworks
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=flat-square&logo=typescript&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Swift](https://img.shields.io/badge/Swift-FA7343?style=flat-square&logo=swift&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-0095D5?style=flat-square&logo=kotlin&logoColor=white)

### Frontend
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=next.js&logoColor=white)
![React Native](https://img.shields.io/badge/React_Native-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Redux](https://img.shields.io/badge/Redux-593D88?style=flat-square&logo=redux&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white)

### Backend & Database
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white)
![GraphQL](https://img.shields.io/badge/GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)

### Cloud & DevOps
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazon-aws&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-0089D0?style=flat-square&logo=microsoft-azure&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)

### AI & Tools
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![Figma](https://img.shields.io/badge/Figma-F24E1E?style=flat-square&logo=figma&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

</div>

---

## 📊 GitHub Analytics

<div align="center">
  <img height="180em" src="https://github-readme-stats.vercel.app/api?username=yourusername&show_icons=true&theme=dracula&include_all_commits=true&count_private=true&title_color=FF69B4&icon_color=FF69B4"/>
  <img height="180em" src="https://github-readme-streak-stats.herokuapp.com/?user=yourusername&theme=dracula&stroke=FF69B4&ring=FF69B4&fire=FF69B4" alt="GitHub Streak" />
</div>

---

## 💻 Code Philosophy

<details>
<summary><b>Clean Architecture</b></summary>

```typescript
// Example: Separation of concerns in React
// hooks/useHealthData.ts
export const useHealthData = (userId: string) => {
  const [data, setData] = useState<HealthData | null>(null);
  const [loading, setLoading] = useState(true);
  
  useEffect(() => {
    fetchHealthData(userId)
      .then(setData)
      .finally(() => setLoading(false));
  }, [userId]);
  
  return { data, loading };
};

// components/HealthDashboard.tsx
export const HealthDashboard: FC = () => {
  const { data, loading } = useHealthData(userId);
  
  if (loading) return <Skeleton />;
  return <DashboardView data={data} />;
};
```

</details>

<details>
<summary><b>Performance First</b></summary>

```javascript
// Example: Optimized API with caching
const getCachedData = async (key, fetchFn, ttl = 3600) => {
  const cached = await redis.get(key);
  if (cached) return JSON.parse(cached);
  
  const fresh = await fetchFn();
  await redis.setex(key, ttl, JSON.stringify(fresh));
  return fresh;
};

// Usage with automatic cache invalidation
router.get('/api/user/:id/patterns', async (req, res) => {
  const data = await getCachedData(
    `patterns:${req.params.id}`,
    () => analyzeUserPatterns(req.params.id),
    3600
  );
  res.json(data);
});
```

</details>

<details>
<summary><b>User-Centric Design</b></summary>

```tsx
// Example: Accessible, responsive component
interface ButtonProps {
  variant: 'primary' | 'secondary';
  loading?: boolean;
  children: React.ReactNode;
  onClick: () => void;
  ariaLabel?: string;
}

export const Button: FC<ButtonProps> = ({ 
  variant, loading, children, onClick, ariaLabel 
}) => (
  <StyledButton
    variant={variant}
    onClick={onClick}
    disabled={loading}
    aria-label={ariaLabel || children}
    aria-busy={loading}
  >
    {loading ? <Spinner /> : children}
  </StyledButton>
);
```

</details>

---

## 🎯 What I Bring to Your Team

- **🚀 Fast Learner:** Built 4 full-stack projects while working full-time
- **💡 Problem Solver:** Focus on user needs and business impact
- **📈 Data-Driven:** Decisions backed by research and metrics
- **🤝 Team Player:** Clear communication and documentation
- **✨ Quality Focus:** Clean code, tested features, scalable architecture

---

## 🌟 Let's Connect!

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-FF69B4?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/hana-pham-601a551b0/)
[![Portfolio](https://img.shields.io/badge/Portfolio-hanapham.com-FF69B4?style=for-the-badge&logo=firefox&logoColor=white)](https://hanapham.com/)
[![Email](https://img.shields.io/badge/Email-Let's_Talk-FF69B4?style=for-the-badge&logo=gmail&logoColor=white)](mailto:the.hanapham@gmail.com)

### 💬 Open to Opportunities In:
`Frontend Engineering` `Full-Stack Development` `React/React Native` `Health Tech` `AI Integration`

</div>

---

<div align="center">

**⭐ Currently seeking Frontend/Software Engineering roles in Sydney or Remote**

</div>

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=FF69B4&height=60&section=footer" width="100%" />
</div>
