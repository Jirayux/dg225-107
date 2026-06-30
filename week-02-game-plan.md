```mermaid
mindmap
    root((Pac-Man))
      Theme
        เขาวงกต
        อาเขตยุค 80
      Mechanics
        เดินในเขาวงกต
        กิน Pellet
        Power Pellet
      Content
         ผีศัตรู 4 ตัว
         ผลไม้โบนัส
      Audience
         ผู้เล่น Casual
      Audio
         เสียงดนตรี
         เสียงตอนกิน Pallet
```

```mermaid
quadrantChart
    title Pac-Man — Feature Prioritization
    x-axis Low Effort --> High Effort
    y-axis Low Impact --> High Impact
    quadrant-1 Quick Wins
    quadrant-2 Major
    quadrant-3 Nice to Have
    quadrant-4 Reconsider
    Maze Movement: [0.3, 0.95]
    Ghost AI: [0.7, 0.9]
    Online Leaderboard: [0.7, 0.3]
    Power Pellets: [0.2, 0.85]
    Fruit Bonuses: [0.3, 0.4]
    Local Co-op: [0.8, 0.75]
    Custom Mazes: [0.9, 0.2]
```

สรุป:

Features สำหรับ MVP (ซ้ายบน และ ขวาบน - High Impact): Maze Movement, Ghost AI, Power Pellets และ Local Co-op ควรนำมาทำเป็น MVP ก่อน เพราะเป็นหัวใจหลักของเกมและให้คุณค่ากับผู้เล่นสูง

Features ที่ควรตัดออกก่อน (ขวาล่าง - High Effort, Low Impact): Custom Mazes และ Online Leaderboard ควรตัดทิ้งหรือเก็บไว้ทำทีหลัง เพราะใช้แรงและเวลาในการทำมาก แต่ไม่ได้ส่งผลกระทบต่อความสนุกหลักของเกมมากนักในระยะเริ่มต้น

```mermaid
gantt
    title Pac-Man - Production Timeline (6 สัปดาห์)
    dateFormat YYYY-MM-DD
  
    section Pre-Production
    Concept & GDD        :done,    c1, 2026-07-06, 5d
  
    section Production
    Maze Movement        :active,  p1, after c1, 5d
    Ghost AI             :         p2, after p1, 7d
    Pellet & Score       :         p3, after p2, 7d
    Local Co-op          :         p4, after p3, 4d
    Alpha Build          :milestone, m_alpha, after p4, 0d
  
    section Post
    QA & Bug Fix         :         q1, after m_alpha, 5d
    Release Build        :milestone, m1, after q1, 0d
```

```

```
