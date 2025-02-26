import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { FaHospital, FaStethoscope, FaAmbulance, FaPhone } from "react-icons/fa";

export default function HospitalPage() {
  return (
    <div className="min-h-screen bg-gray-100">
      {/* Encabezado */}
      <header className="bg-blue-600 text-white p-5 text-center text-2xl font-bold flex items-center justify-center gap-2">
        <FaHospital /> Hospital San José
      </header>

      {/* Sección de Bienvenida */}
      <section className="p-10 text-center">
        <h1 className="text-3xl font-semibold text-gray-800">Bienvenidos a Hospital San José</h1>
        <p className="mt-3 text-gray-600">Brindando atención médica de calidad con tecnología avanzada y un equipo profesional.</p>
      </section>

      {/* Servicios */}
      <div className="grid md:grid-cols-3 gap-6 px-10">
        <Card className="bg-white p-5 shadow-lg text-center">
          <CardContent>
            <FaStethoscope className="text-blue-600 text-4xl mx-auto mb-3" />
            <h2 className="text-xl font-semibold">Consultas Médicas</h2>
            <p className="text-gray-600">Atención personalizada con especialistas en diversas áreas.</p>
          </CardContent>
        </Card>
        
        <Card className="bg-white p-5 shadow-lg text-center">
          <CardContent>
            <FaAmbulance className="text-red-600 text-4xl mx-auto mb-3" />
            <h2 className="text-xl font-semibold">Emergencias</h2>
            <p className="text-gray-600">Servicio de urgencias 24/7 con respuesta inmediata.</p>
          </CardContent>
        </Card>
      </div>

      {/* Contacto */}
      <footer className="bg-blue-600 text-white p-5 mt-10 text-center flex flex-col items-center">
        <FaPhone className="text-2xl mb-2" />
        <p>Contacto: +57 123 456 7890</p>
        <p>Dirección: Calle 123, Ciudad</p>
      </footer>
    </div>
  );
}
