"use client"

import { Badge } from "@/components/ui/badge"
import { Card, CardContent } from "@/components/ui/card"
import { Button } from "@/components/ui/button"
import {
  Code2,
  Database,
  Server,
  Shield,
  Zap,
  Mail,
  Github,
  Linkedin,
  ExternalLink,
  CheckCircle,
  Sparkles,
  Rocket,
  Brain,
} from "lucide-react"

export default function Component() {
  const techStack = [
    { name: "Java 17", category: "language", color: "bg-orange-500" },
    { name: "Spring Boot", category: "framework", color: "bg-green-500" },
    { name: "Spring Security", category: "framework", color: "bg-green-600" },
    { name: "PostgreSQL", category: "database", color: "bg-blue-500" },
    { name: "MySQL", category: "database", color: "bg-blue-600" },
    { name: "JWT", category: "auth", color: "bg-purple-500" },
    { name: "WebSocket", category: "realtime", color: "bg-indigo-500" },
    { name: "Docker", category: "devops", color: "bg-cyan-500" },
    { name: "Linux", category: "os", color: "bg-gray-600" },
    { name: "Git", category: "tool", color: "bg-red-500" },
    { name: "Swagger", category: "api", color: "bg-yellow-500" },
    { name: "Telegram Bot API", category: "bot", color: "bg-blue-400" },
  ]

  const skills = [
    {
      icon: <Code2 className="w-5 h-5" />,
      title: "Toza va saqlash mumkin bo'lgan backend kod yozish",
      description: "SOLID prinsiplariga amal qilgan holda",
    },
    {
      icon: <Shield className="w-5 h-5" />,
      title: "JWT + Spring Security bilan xavfsizlik",
      description: "Zamonaviy autentifikatsiya va avtorizatsiya",
    },
    {
      icon: <Zap className="w-5 h-5" />,
      title: "WebSocket bilan real-time tizimlar",
      description: "Asinxron va tezkor ma'lumot almashinuvi",
    },
    {
      icon: <Brain className="w-5 h-5" />,
      title: "Murakkab mantiqli Telegram botlar",
      description: "Keng imkoniyatli bot arxitekturasi",
    },
    {
      icon: <Server className="w-5 h-5" />,
      title: "Swagger orqali API hujjatlash",
      description: "Professional API dokumentatsiyasi",
    },
    {
      icon: <Database className="w-5 h-5" />,
      title: "MultipartFile orqali fayl yuklash",
      description: "Xavfsiz fayl boshqaruv tizimi",
    },
  ]

  return (
    <div className="min-h-screen bg-gradient-to-br from-slate-900 via-purple-900 to-slate-900">
      {/* Hero Section */}
      <div className="relative overflow-hidden">
        <div className="absolute inset-0 bg-gradient-to-r from-purple-600/20 to-cyan-600/20" />
        <div className="relative max-w-6xl mx-auto px-6 py-16">
          <div className="text-center space-y-6">
            <div className="inline-flex items-center gap-2 px-4 py-2 bg-white/10 backdrop-blur-sm rounded-full border border-white/20">
              <Sparkles className="w-4 h-4 text-yellow-400" />
              <span className="text-sm text-white/90">2025 Zamonaviy Dizayn</span>
            </div>

            <h1 className="text-5xl md:text-7xl font-bold bg-gradient-to-r from-white via-purple-200 to-cyan-200 bg-clip-text text-transparent">
              Salom, men Alisher Nayimov 👋
            </h1>

            <div className="flex flex-wrap justify-center gap-3 text-lg md:text-xl text-white/80">
              <Badge
                variant="secondary"
                className="bg-white/10 text-white border-white/20 hover:bg-white/20 transition-colors"
              >
                Java Backend Developer
              </Badge>
              <Badge
                variant="secondary"
                className="bg-white/10 text-white border-white/20 hover:bg-white/20 transition-colors"
              >
                Spring Boot Mutaxassisi
              </Badge>
              <Badge
                variant="secondary"
                className="bg-white/10 text-white border-white/20 hover:bg-white/20 transition-colors"
              >
                Telegram Bot Arxitekti
              </Badge>
            </div>

            <div className="flex justify-center gap-4 pt-4">
              <Button className="bg-gradient-to-r from-purple-600 to-cyan-600 hover:from-purple-700 hover:to-cyan-700 text-white border-0">
                <Mail className="w-4 h-4 mr-2" />
                Bog'lanish
              </Button>
              <Button variant="outline" className="border-white/20 text-white hover:bg-white/10 bg-transparent">
                <Github className="w-4 h-4 mr-2" />
                GitHub
              </Button>
            </div>
          </div>
        </div>
      </div>

      {/* About Section */}
      <div className="max-w-6xl mx-auto px-6 py-16">
        <Card className="bg-white/5 backdrop-blur-sm border-white/10 hover:bg-white/10 transition-all duration-300">
          <CardContent className="p-8">
            <div className="grid md:grid-cols-2 gap-8 items-center">
              <div className="space-y-6">
                <div className="flex items-center gap-3">
                  <Rocket className="w-8 h-8 text-purple-400" />
                  <h2 className="text-3xl font-bold text-white">Men haqimda</h2>
                </div>

                <div className="space-y-4 text-white/80 leading-relaxed">
                  <p className="flex items-start gap-3">
                    <span className="text-purple-400 mt-1">🎓</span>
                    <span>
                      <strong className="text-white">PDP Academy</strong>da o'qidim va{" "}
                      <strong className="text-purple-300">Java Backend Development</strong>ga ixtisoslashtim.
                    </span>
                  </p>

                  <p className="flex items-start gap-3">
                    <span className="text-cyan-400 mt-1">🏗️</span>
                    <span>
                      <strong className="text-cyan-300">Spring Boot, PostgreSQL, JWT</strong> va{" "}
                      <strong className="text-cyan-300">WebSocket</strong> texnologiyalari yordamida backend tizimlar
                      quraman.
                    </span>
                  </p>

                  <p className="flex items-start gap-3">
                    <span className="text-green-400 mt-1">🤖</span>
                    <span>
                      Kuchli <strong className="text-green-300">Telegram Botlar</strong> yarataman va xavfsiz{" "}
                      <strong className="text-green-300">REST API</strong>lar ishlab chiqaraman.
                    </span>
                  </p>

                  <p className="flex items-start gap-3">
                    <span className="text-orange-400 mt-1">🐧</span>
                    <span>
                      <strong className="text-orange-300">Linux</strong> va{" "}
                      <strong className="text-orange-300">Docker</strong> bilan ishlayman, development workflow'imda
                      foydalanaman.
                    </span>
                  </p>
                </div>
              </div>

              <div className="relative">
                <div className="absolute inset-0 bg-gradient-to-r from-purple-600/20 to-cyan-600/20 rounded-2xl blur-xl" />
                <img
                  src="/placeholder.svg?height=300&width=400"
                  alt="Developer workspace"
                  className="relative rounded-2xl shadow-2xl border border-white/10"
                />
              </div>
            </div>
          </CardContent>
        </Card>
      </div>

      {/* Tech Stack */}
      <div className="max-w-6xl mx-auto px-6 py-16">
        <div className="text-center mb-12">
          <h2 className="text-4xl font-bold text-white mb-4">🛠️ Texnologik Stack</h2>
          <p className="text-white/60 text-lg">Men ishlatadigan zamonaviy texnologiyalar</p>
        </div>

        <div className="grid grid-cols-2 md:grid-cols-4 lg:grid-cols-6 gap-4">
          {techStack.map((tech, index) => (
            <Card
              key={index}
              className="bg-white/5 backdrop-blur-sm border-white/10 hover:bg-white/10 hover:scale-105 transition-all duration-300 group"
            >
              <CardContent className="p-4 text-center">
                <div
                  className={`w-3 h-3 ${tech.color} rounded-full mx-auto mb-3 group-hover:scale-110 transition-transform`}
                />
                <p className="text-white font-medium text-sm">{tech.name}</p>
                <p className="text-white/50 text-xs mt-1 capitalize">{tech.category}</p>
              </CardContent>
            </Card>
          ))}
        </div>
      </div>

      {/* Skills */}
      <div className="max-w-6xl mx-auto px-6 py-16">
        <div className="text-center mb-12">
          <h2 className="text-4xl font-bold text-white mb-4">🧠 Eng yaxshi bilgan narsalarim</h2>
          <p className="text-white/60 text-lg">Professional ko'nikmalarim va tajribam</p>
        </div>

        <div className="grid md:grid-cols-2 lg:grid-cols-3 gap-6">
          {skills.map((skill, index) => (
            <Card
              key={index}
              className="bg-white/5 backdrop-blur-sm border-white/10 hover:bg-white/10 transition-all duration-300 group"
            >
              <CardContent className="p-6">
                <div className="flex items-start gap-4">
                  <div className="p-3 bg-gradient-to-r from-purple-600/20 to-cyan-600/20 rounded-lg group-hover:from-purple-600/30 group-hover:to-cyan-600/30 transition-colors">
                    <div className="text-purple-300 group-hover:text-purple-200 transition-colors">{skill.icon}</div>
                  </div>
                  <div className="flex-1">
                    <div className="flex items-center gap-2 mb-2">
                      <CheckCircle className="w-4 h-4 text-green-400" />
                      <h3 className="text-white font-semibold text-sm leading-tight">{skill.title}</h3>
                    </div>
                    <p className="text-white/60 text-sm">{skill.description}</p>
                  </div>
                </div>
              </CardContent>
            </Card>
          ))}
        </div>
      </div>

      {/* Contact */}
      <div className="max-w-6xl mx-auto px-6 py-16">
        <Card className="bg-gradient-to-r from-purple-600/10 to-cyan-600/10 backdrop-blur-sm border-white/10">
          <CardContent className="p-8 text-center">
            <h2 className="text-3xl font-bold text-white mb-4">📞 Men bilan bog'laning</h2>
            <p className="text-white/70 mb-8 text-lg">Loyihalar va hamkorlik uchun</p>

            <div className="flex flex-wrap justify-center gap-4">
              <Button className="bg-gradient-to-r from-purple-600 to-purple-700 hover:from-purple-700 hover:to-purple-800 text-white">
                <Mail className="w-4 h-4 mr-2" />
                nayimovalisher2001@gmail.com
              </Button>

              <Button variant="outline" className="border-white/20 text-white hover:bg-white/10 bg-transparent">
                <Github className="w-4 h-4 mr-2" />
                GitHub Profile
                <ExternalLink className="w-3 h-3 ml-2" />
              </Button>

              <Button variant="outline" className="border-white/20 text-white hover:bg-white/10 bg-transparent">
                <Linkedin className="w-4 h-4 mr-2" />
                LinkedIn
                <ExternalLink className="w-3 h-3 ml-2" />
              </Button>
            </div>
          </CardContent>
        </Card>
      </div>

      {/* Footer */}
      <div className="text-center py-8 border-t border-white/10">
        <p className="text-white/50">✨ 2025 yilgi zamonaviy dizayn bilan yaratilgan | Alisher Nayimov</p>
      </div>
    </div>
  )
}
