#Mokshda's Portfolio

import Link from "next/link"
import { Button } from "@/components/ui/button"
import { Card, CardContent, CardHeader, CardTitle } from "@/components/ui/card"
import { Badge } from "@/components/ui/badge"
import {
  BarChart3,
  BookOpen,
  BriefcaseBusiness,
  Download,
  GraduationCap,
  Linkedin,
  Mail,
  MapPin,
  Phone,
  Trophy,
  User,
} from "lucide-react"

export default function DashboardTemplate() {
  return (
    <div className="min-h-screen bg-gray-50">
      {/* Sidebar */}
      <div className="fixed inset-y-0 left-0 z-10 hidden w-64 bg-white border-r lg:block">
        <div className="flex flex-col h-full">
          <div className="p-6 border-b">
            <h1 className="text-xl font-bold">Mokshda Sharma</h1>
            <p className="text-sm text-gray-500">Data Analytics Professional</p>
          </div>
          <nav className="flex-1 p-4 space-y-1 overflow-auto">
            <Link href="#about" className="flex items-center px-3 py-2 text-sm rounded-md hover:bg-gray-100">
              <User className="w-4 h-4 mr-2" />
              About
            </Link>
            <Link href="#experience" className="flex items-center px-3 py-2 text-sm rounded-md hover:bg-gray-100">
              <BriefcaseBusiness className="w-4 h-4 mr-2" />
              Experience
            </Link>
            <Link href="#projects" className="flex items-center px-3 py-2 text-sm rounded-md hover:bg-gray-100">
              <BookOpen className="w-4 h-4 mr-2" />
              Projects
            </Link>
            <Link href="#education" className="flex items-center px-3 py-2 text-sm rounded-md hover:bg-gray-100">
              <GraduationCap className="w-4 h-4 mr-2" />
              Education
            </Link>
            <Link href="#skills" className="flex items-center px-3 py-2 text-sm rounded-md hover:bg-gray-100">
              <BarChart3 className="w-4 h-4 mr-2" />
              Skills
            </Link>
            <Link href="#honors" className="flex items-center px-3 py-2 text-sm rounded-md hover:bg-gray-100">
              <Trophy className="w-4 h-4 mr-2" />
              Honors
            </Link>
          </nav>
          <div className="p-4 border-t">
            <div className="flex flex-col space-y-2">
              <Link
                href="mailto:mokshda879@gmail.com"
                className="flex items-center text-sm text-gray-500 hover:text-gray-900"
              >
                <Mail className="w-4 h-4 mr-2" />
                mokshda879@gmail.com
              </Link>
              <Link href="tel:7657670302" className="flex items-center text-sm text-gray-500 hover:text-gray-900">
                <Phone className="w-4 h-4 mr-2" />
                (765) 767-0302
              </Link>
              <Link
                href="https://www.linkedin.com/in/mokshda-sharma-b740a7165"
                target="_blank"
                rel="noopener noreferrer"
                className="flex items-center text-sm text-gray-500 hover:text-gray-900"
              >
                <Linkedin className="w-4 h-4 mr-2" />
                LinkedIn
              </Link>
            </div>
          </div>
        </div>
      </div>
