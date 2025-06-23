import React from "react";
import { Button } from "@/components/ui/button";
import { Card, CardContent } from "@/components/ui/card";
import { ShieldCheck, PhoneCall, MapPin } from "lucide-react";

export default function QuietRoomHome() {
  return (
    <div className="min-h-screen bg-gradient-to-br from-purple-100 to-pink-200 p-6 flex flex-col items-center justify-center">
      <header className="text-center mb-10">
        <h1 className="text-5xl font-bold text-purple-800">Quiet Room</h1>
        <p className="text-lg mt-2 text-purple-600">Ensuring Women’s Safety, Anytime, Anywhere</p>
      </header>

      <section className="grid md:grid-cols-3 gap-6 max-w-6xl w-full">
        <Card className="bg-white rounded-2xl shadow-xl p-6 hover:scale-105 transition-all">
          <CardContent className="text-center">
            <ShieldCheck className="mx-auto text-purple-700" size={40} />
            <h2 className="text-xl font-semibold mt-4">Emergency Alert</h2>
            <p className="mt-2 text-sm text-gray-600">Send instant alerts to your emergency contacts with just one tap.</p>
          </CardContent>
        </Card>

        <Card className="bg-white rounded-2xl shadow-xl p-6 hover:scale-105 transition-all">
          <CardContent className="text-center">
            <PhoneCall className="mx-auto text-purple-700" size={40} />
            <h2 className="text-xl font-semibold mt-4">24/7 Support</h2>
            <p className="mt-2 text-sm text-gray-600">Connect with our verified support team any time, day or night.</p>
          </CardContent>
        </Card>

        <Card className="bg-white rounded-2xl shadow-xl p-6 hover:scale-105 transition-all">
          <CardContent className="text-center">
            <MapPin className="mx-auto text-purple-700" size={40} />
            <h2 className="text-xl font-semibold mt-4">Live Location Sharing</h2>
            <p className="mt-2 text-sm text-gray-600">Share your live location with trusted contacts during travel or emergencies.</p>
          </CardContent>
        </Card>
      </section>

      <div className="mt-12 text-center">
        <h3 className="text-2xl font-bold text-purple-800 mb-4">Download the Quiet Room App</h3>
        <Button className="bg-purple-700 hover:bg-purple-800 text-white px-6 py-3 rounded-2xl text-lg shadow-md">
          Get the App
        </Button>
      </div>
    </div>
  );
}
