import React from "react";
import { Button } from "@/components/ui/button";
import { Card, CardContent } from "@/components/ui/card";
import { Mail, Phone } from "lucide-react";

export default function Home() {
  return (
    <div className="min-h-screen bg-gray-100">
      {/* Header */}
      <header className="bg-blue-600 text-white py-4 px-6 flex justify-between items-center">
        <h1 className="text-2xl font-bold">Nexa Soluções e Serviços</h1>
        <Button variant="outline" className="border-white text-white">Contato</Button>
      </header>
      
      {/* Hero Section */}
      <section className="text-center py-20 bg-blue-500 text-white">
        <h2 className="text-4xl font-bold">Construção Rápida, Eficiente e Inovadora</h2>
        <p className="mt-4 text-lg">Transformamos projetos em realidade com tecnologia e excelência.</p>
        <Button className="mt-6 bg-white text-blue-600 px-6 py-3">Saiba Mais</Button>
      </section>

      {/* Sobre Nós */}
      <section className="py-16 px-6 text-center">
        <h2 className="text-3xl font-bold">Sobre a Nexa</h2>
        <p className="mt-4 text-gray-700 max-w-2xl mx-auto">
          A Nexa é líder em soluções inovadoras para construção modular e métodos construtivos eficientes.
        </p>
      </section>

      {/* Serviços */}
      <section className="bg-gray-200 py-16 px-6 text-center">
        <h2 className="text-3xl font-bold">Nossos Serviços</h2>
        <div className="mt-6 grid grid-cols-1 md:grid-cols-3 gap-6 max-w-5xl mx-auto">
          <Card>
            <CardContent className="p-6 text-center">
              <h3 className="text-xl font-semibold">Construção Modular</h3>
              <p className="text-gray-600">Eficiência e rapidez com tecnologia de ponta.</p>
            </CardContent>
          </Card>
          <Card>
            <CardContent className="p-6 text-center">
              <h3 className="text-xl font-semibold">Projetos Personalizados</h3>
              <p className="text-gray-600">Soluções adaptadas às necessidades de cada cliente.</p>
            </CardContent>
          </Card>
          <Card>
            <CardContent className="p-6 text-center">
              <h3 className="text-xl font-semibold">Gestão de Obras</h3>
              <p className="text-gray-600">Planejamento e execução para máxima eficiência.</p>
            </CardContent>
          </Card>
        </div>
      </section>

      {/* Contato */}
      <section className="py-16 px-6 text-center">
        <h2 className="text-3xl font-bold">Entre em Contato</h2>
        <p className="mt-4 text-gray-700">Fale conosco para saber mais sobre nossos serviços.</p>
        <div className="mt-6 flex flex-col items-center gap-4">
          <p className="flex items-center gap-2 text-lg"><Mail className="w-5 h-5" /> contato@nexa.com</p>
          <p className="flex items-center gap-2 text-lg"><Phone className="w-5 h-5" /> (99) 99999-9999</p>
        </div>
      </section>

      {/* Footer */}
      <footer className="bg-blue-600 text-white text-center py-4">
        <p>&copy; 2025 Nexa Soluções e Serviços - Todos os direitos reservados.</p>
      </footer>
    </div>
  );
}
