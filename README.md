import React, { useEffect, useState } from "react";
import { Code2, PieChart, Database, Cloud } from "lucide-react";

const skills = [
  { label: "PYTHON", lvl: 8, icon: Code2, color: "#7dd3ff" },
  { label: "PANDAS", lvl: 7, icon: PieChart, color: "#c77dff" },
  { label: "SQL", lvl: 6, icon: Database, color: "#ff9ecf" },
  { label: "AWS", lvl: 2, icon: Cloud, color: "#7c3aed" },
];

const floaters = [
  { top: "6%", left: "4%", size: 8, color: "#7dd3ff", delay: 0 },
  { top: "3%", left: "50%", size: 4, color: "#c77dff", delay: 0.6 },
  { top: "8%", left: "94%", size: 6, color: "#ec4899", delay: 1.1 },
  { top: "80%", left: "10%", size: 5, color: "#c77dff", delay: 0.3 },
  { top: "88%", left: "40%", size: 3, color: "#7dd3ff", delay: 1.5 },
  { top: "84%", left: "88%", size: 5, color: "#ec4899", delay: 0.8 },
];

export default function GamingProfileHero() {
  const [xp, setXp] = useState(0);

  useEffect(() => {
    const t = setTimeout(() => setXp(80), 300);
    return () => clearTimeout(t);
  }, []);

  return (
    <div
      style={{
        position: "relative",
        overflow: "hidden",
        borderRadius: "16px",
        minHeight: "360px",
        padding: "48px 32px",
        background:
          "repeating-linear-gradient(0deg, #0d0a1f, #0d0a1f 2px, #100c24 2px, #100c24 4px)",
        fontFamily: "'Cascadia Code','Fira Code',Consolas,monospace",
      }}
    >
      <style>{`
        @keyframes floatY {
          0%, 100% { transform: translateY(0px); opacity: 0.5; }
          50% { transform: translateY(-14px); opacity: 1; }
        }
        @keyframes glowPulse {
          0%, 100% { filter: drop-shadow(0 0 6px rgba(199,125,255,0.5)); }
          50% { filter: drop-shadow(0 0 16px rgba(236,72,153,0.7)); }
        }
      `}</style>

      {floaters.map((f, i) => (
        <div
          key={i}
          style={{
            position: "absolute",
            top: f.top,
            left: f.left,
            width: f.size,
            height: f.size,
            background: f.color,
            borderRadius: i % 2 === 0 ? "2px" : "50%",
            animation: `floatY ${3 + i * 0.4}s ease-in-out infinite`,
            animationDelay: `${f.delay}s`,
          }}
        />
      ))}

      <div
        style={{
          position: "absolute",
          top: "40%",
          left: "5%",
          width: "26px",
          height: "26px",
          opacity: 0.85,
          animation: "floatY 4s ease-in-out infinite",
        }}
      >
        <div style={{ position: "absolute", top: "9px", left: "0", width: "26px", height: "8px", background: "#c9b6ea", borderRadius: "2px" }} />
        <div style={{ position: "absolute", top: "0", left: "9px", width: "8px", height: "26px", background: "#c9b6ea", borderRadius: "2px" }} />
      </div>

      <div style={{ position: "relative", zIndex: 2, textAlign: "center" }}>
        <h1
          style={{
            fontSize: "56px",
            fontWeight: 800,
            letterSpacing: "6px",
            margin: 0,
            backgroundImage: "linear-gradient(90deg, #7dd3ff, #c77dff, #ec4899)",
            WebkitBackgroundClip: "text",
            WebkitTextFillColor: "transparent",
            animation: "glowPulse 3s ease-in-out infinite",
          }}
        >
          SHREYA.EXE
        </h1>

        <p
          style={{
            color: "#c9b6ea",
            fontSize: "16px",
            letterSpacing: "4px",
            marginTop: "14px",
            fontWeight: 600,
          }}
        >
          DATA ENGINEER · LEVEL: FINAL YEAR
        </p>

        <div style={{ maxWidth: "440px", margin: "32px auto 0", textAlign: "left" }}>
          <span style={{ color: "#7dd3ff", fontSize: "13px", letterSpacing: "2px" }}>XP</span>
          <div
            style={{
              marginTop: "6px",
              width: "100%",
              height: "16px",
              borderRadius: "8px",
              background: "#1a1030",
              border: "1px solid #3a2560",
              position: "relative",
              overflow: "hidden",
            }}
          >
            <div
              style={{
                height: "100%",
                width: `${xp}%`,
                borderRadius: "8px",
                background: "linear-gradient(90deg, #3b5bfd, #7c3aed, #ec4899)",
                transition: "width 1.6s ease-out",
              }}
            />
          </div>
          <span style={{ color: "#c9b6ea", fontSize: "12px", float: "right", marginTop: "4px" }}>{xp}%</span>
        </div>

        <div
          style={{
            display: "grid",
            gridTemplateColumns: "1fr 1fr",
            gap: "10px 40px",
            maxWidth: "440px",
            margin: "40px auto 0",
            textAlign: "left",
          }}
        >
          {skills.map((s, i) => {
            const Icon = s.icon;
            return (
              <div key={i} style={{ display: "flex", alignItems: "center", gap: "10px" }}>
                <Icon size={16} color={s.color} />
                <span style={{ color: "#e9d8fd", fontSize: "14px", letterSpacing: "1px" }}>
                  {s.label} <span style={{ color: "#c9b6ea" }}>Lv.{s.lvl}</span>
                </span>
              </div>
            );
          })}
        </div>
      </div>
    </div>
  );
}
