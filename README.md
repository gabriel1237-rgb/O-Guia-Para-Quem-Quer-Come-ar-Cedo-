# O-Guia-Para-Quem-Quer-Come-ar-Cedo-
Aprenda a prosperar cedo
import React from 'react';
import { ArrowRight, Clock, Target, Lightbulb, TrendingUp, BookOpen, Users, Star } from 'lucide-react';
import { Button } from '@/components/ui/button';
import { Card, CardContent, CardDescription, CardHeader, CardTitle } from '@/components/ui/card';

const Index = () => {
  const benefits = [
    {
      icon: <Clock className="w-8 h-8 text-blue-600" />,
      title: "Mais Tempo para Crescer",
      description: "Começar cedo significa ter mais tempo para desenvolver habilidades, construir experiência e corrigir erros."
    },
    {
      icon: <Target className="w-8 h-8 text-green-600" />,
      title: "Foco e Disciplina",
      description: "Desenvolva hábitos produtivos e disciplina pessoal que serão fundamentais para o sucesso."
    },
    {
      icon: <TrendingUp className="w-8 h-8 text-purple-600" />,
      title: "Vantagem Competitiva",
      description: "Quem começa cedo tem uma vantagem significativa no mercado de trabalho e nos negócios."
    }
  ];

  const steps = [
    {
      number: "01",
      title: "Defina Seus Objetivos",
      description: "Estabeleça metas claras e específicas para os próximos 1, 3 e 5 anos."
    },
    {
      number: "02",
      title: "Desenvolva Habilidades",
      description: "Invista em aprendizado contínuo e desenvolva competências valiosas para o mercado."
    },
    {
      number: "03",
      title: "Construa Sua Rede",
      description: "Conecte-se com pessoas da sua área e construa relacionamentos profissionais sólidos."
    },
    {
      number: "04",
      title: "Pratique e Aplique",
      description: "Coloque o conhecimento em prática através de projetos, estágios ou empreendimentos."
    }
  ];

  const tips = [
    {
      icon: <BookOpen className="w-6 h-6" />,
      title: "Leia Constantemente",
      description: "Dedique pelo menos 30 minutos por dia para leitura de livros e artigos relevantes."
    },
    {
      icon: <Users className="w-6 h-6" />,
      title: "Encontre Mentores",
      description: "Busque pessoas experientes que possam te orientar e compartilhar conhecimento."
    },
    {
      icon: <Lightbulb className="w-6 h-6" />,
      title: "Seja Curioso",
      description: "Mantenha sempre a mente aberta para aprender coisas novas e questionar o status quo."
    },
    {
      icon: <Star className="w-6 h-6" />,
      title: "Celebre Pequenas Vitórias",
      description: "Reconheça e celebre cada progresso, por menor que seja, para manter a motivação."
    }
  ];

  return (
    <div className="min-h-screen bg-gradient-to-br from-blue-50 via-white to-green-50">
      {/* Hero Section */}
      <section className="relative py-20 px-6 text-center">
        <div className="max-w-4xl mx-auto">
          <h1 className="text-5xl md:text-6xl font-bold text-gray-900 mb-6 leading-tight">
            O Guia Para Quem Quer{" "}
            <span className="bg-gradient-to-r from-blue-600 to-green-600 bg-clip-text text-transparent">
              Começar Cedo
            </span>
          </h1>
          <p className="text-xl text-gray-600 mb-8 max-w-2xl mx-auto">
            Descubra como dar os primeiros passos rumo ao sucesso e construir uma carreira sólida desde jovem.
            Não espere pelo momento perfeito - comece agora!
          </p>
          <Button size="lg" className="bg-gradient-to-r from-blue-600 to-green-600 hover:from-blue-700 hover:to-green-700 text-white px-8 py-3 rounded-full shadow-lg hover:shadow-xl transition-all duration-300">
            Começar Minha Jornada
            <ArrowRight className="ml-2 w-5 h-5" />
          </Button>
        </div>
      </section>

      {/* Benefits Section */}
      <section className="py-16 px-6">
        <div className="max-w-6xl mx-auto">
          <h2 className="text-3xl font-bold text-center text-gray-900 mb-12">
            Por Que Começar Cedo Faz Diferença?
          </h2>
          <div className="grid md:grid-cols-3 gap-8">
            {benefits.map((benefit, index) => (
              <Card key={index} className="text-center border-0 shadow-lg hover:shadow-xl transition-all duration-300 hover:-translate-y-2">
                <CardHeader>
                  <div className="flex justify-center mb-4">
                    {benefit.icon}
                  </div>
                  <CardTitle className="text-xl">{benefit.title}</CardTitle>
                </CardHeader>
                <CardContent>
                  <CardDescription className="text-gray-600 leading-relaxed">
                    {benefit.description}
                  </CardDescription>
                </CardContent>
              </Card>
            ))}
          </div>
        </div>
      </section>

      {/* Steps Section */}
      <section className="py-16 px-6 bg-gray-50">
        <div className="max-w-6xl mx-auto">
          <h2 className="text-3xl font-bold text-center text-gray-900 mb-12">
            4 Passos Para Começar
          </h2>
          <div className="grid md:grid-cols-2 gap-8">
            {steps.map((step, index) => (
              <div key={index} className="flex items-start space-x-4 p-6 bg-white rounded-xl shadow-md hover:shadow-lg transition-all duration-300">
                <div className="flex-shrink-0">
                  <div className="w-12 h-12 bg-gradient-to-r from-blue-600 to-green-600 text-white rounded-full flex items-center justify-center font-bold text-lg">
                    {step.number}
                  </div>
                </div>
                <div>
                  <h3 className="text-xl font-semibold text-gray-900 mb-2">{step.title}</h3>
                  <p className="text-gray-600 leading-relaxed">{step.description}</p>
                </div>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* Tips Section */}
      <section className="py-16 px-6">
        <div className="max-w-6xl mx-auto">
          <h2 className="text-3xl font-bold text-center text-gray-900 mb-12">
            Dicas Práticas Para o Sucesso
          </h2>
          <div className="grid md:grid-cols-2 lg:grid-cols-4 gap-6">
            {tips.map((tip, index) => (
              <Card key={index} className="border-0 shadow-md hover:shadow-lg transition-all duration-300 hover:-translate-y-1">
                <CardHeader className="pb-3">
                  <div className="w-12 h-12 bg-gradient-to-r from-blue-100 to-green-100 rounded-lg flex items-center justify-center mb-3">
                    <div className="text-blue-600">
                      {tip.icon}
                    </div>
                  </div>
                  <CardTitle className="text-lg">{tip.title}</CardTitle>
                </CardHeader>
                <CardContent>
                  <CardDescription className="text-gray-600 text-sm leading-relaxed">
                    {tip.description}
                  </CardDescription>
                </CardContent>
              </Card>
            ))}
          </div>
        </div>
      </section>

      {/* CTA Section */}
      <section className="py-16 px-6 bg-gradient-to-r from-blue-600 to-green-600">
        <div className="max-w-4xl mx-auto text-center">
          <h2 className="text-3xl font-bold text-white mb-6">
            Pronto Para Começar Sua Jornada?
          </h2>
          <p className="text-xl text-blue-100 mb-8">
            O tempo perfeito para plantar uma árvore foi há 20 anos. O segundo melhor tempo é agora.
          </p>
          <Button size="lg" variant="secondary" className="bg-white text-blue-600 hover:bg-gray-100 px-8 py-3 rounded-full shadow-lg hover:shadow-xl transition-all duration-300">
            Comece Hoje Mesmo
            <ArrowRight className="ml-2 w-5 h-5" />
          </Button>
        </div>
      </section>

      {/* Footer */}
      <footer className="py-8 px-6 bg-gray-900 text-gray-400 text-center">
        <p>© 2024 Guia Para Começar Cedo. Construindo futuros de sucesso, um passo de cada vez.</p>
      </footer>
    </div>
  );
};

export default Index;
