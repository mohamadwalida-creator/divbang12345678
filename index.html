import React, { useState } from "react";
import {
  ResponsiveContainer,
  LineChart,
  Line,
  BarChart,
  Bar,
  XAxis,
  YAxis,
  Tooltip,
  CartesianGrid,
  PieChart,
  Pie,
  Cell,
  Legend as RLegend,
} from "recharts";
import { Trophy, Layers, Target, Wallet, Sparkles, CheckCircle2 } from "lucide-react";

const ink = "#1F2430";
const inkSoft = "#6B7280";
const border = "#E4E1D8";

/* ---------- Data riil: Kontrak Manajemen 2026, realisasi s.d. Juli 2026 ---------- */

const metricBlocks = [
  { icon: Trophy, label: "Total nilai kinerja", value: "106,80", sub: "dari basis 100", color: "#5B3FA8" },
  { icon: Layers, label: "Skor kategori KPI (A)", value: "43,50", sub: "bobot 40", color: "#7A3FA8" },
  { icon: Target, label: "Skor performance (B)", value: "63,30", sub: "bobot 60", color: "#B23FA0" },
  { icon: Wallet, label: "Pendapatan service fee", value: "Rp 398,56 M", sub: "capaian 105,0%", color: "#2FA097" },
  { icon: Sparkles, label: "Pendapatan inovatif", value: "Rp 4.056,68 M", sub: "capaian 110,0%", color: "#2E8C7E" },
  { icon: CheckCircle2, label: "Indikator capai target", value: "15 / 15", sub: "100% indikator", color: "#0F6E56" },
];

const serviceFee = [
  { bulan: "Jan", target: 49.26, realisasi: 42.94 },
  { bulan: "Feb", target: 98.52, realisasi: 94.68 },
  { bulan: "Mar", target: 147.77, realisasi: 146.71 },
  { bulan: "Apr", target: 197.03, realisasi: 202.49 },
  { bulan: "Mei", target: 246.29, realisasi: 261.05 },
  { bulan: "Jun", target: 295.55, realisasi: 332.11 },
  { bulan: "Jul", target: 379.42, realisasi: 398.56 },
];

const pendapatanInovatif = [
  { bulan: "Jan", target: 190, realisasi: 192.31 },
  { bulan: "Feb", target: 681.11, realisasi: 681.11 },
  { bulan: "Mar", target: 1099.65, realisasi: 1099.65 },
  { bulan: "Apr", target: 1712.92, realisasi: 1743.55 },
  { bulan: "Mei", target: 2178.65, realisasi: 2557.76 },
  { bulan: "Jun", target: 2414.4, realisasi: 2972.04 },
  { bulan: "Jul", target: 3268, realisasi: 4056.68 },
];

const efisiensiEnergi = [
  { bulan: "Jan", target: 0.09, realisasi: 0.09 },
  { bulan: "Feb", target: 6.42, realisasi: 9.83 },
  { bulan: "Mar", target: 9.63, realisasi: 10.88 },
  { bulan: "Apr", target: 13.03, realisasi: 13.03 },
  { bulan: "Mei", target: 13.18, realisasi: 13.18 },
  { bulan: "Jun", target: 19.5, realisasi: 23.35 },
  { bulan: "Jul", target: 21.88, realisasi: 28.49 },
];

const indikator = [
  { kategori: "A", nama: "Pendapatan service fee", satuan: "Rp Miliar", bobot: 10, target: "379,42", realisasi: "398,56", pct: 105.0 },
  { kategori: "A", nama: "Pengendalian anggaran operasi", satuan: "% penyerapan", bobot: 10, target: "58,0", realisasi: "15,2", pct: 110.0 },
  { kategori: "A", nama: "Pendapatan inovatif", satuan: "Rp Miliar", bobot: 10, target: "3.268,0", realisasi: "4.056,7", pct: 110.0 },
  { kategori: "A", nama: "Efisiensi pengelolaan energi primer", satuan: "Rp Miliar", bobot: 10, target: "21,88", realisasi: "28,49", pct: 130.2 },
  { kategori: "B", nama: "Pasokan batubara — tambang sendiri & afiliasi", satuan: "Ribu MT", bobot: 4, target: "467,5", realisasi: "541,6", pct: 110.0 },
  { kategori: "B", nama: "Pasokan batubara — ke Coal Blending Facility", satuan: "Ribu MT", bobot: 4, target: "350,0", realisasi: "359,5", pct: 102.7 },
  { kategori: "B", nama: "Pasokan batubara — ke Intermediate Stockpile", satuan: "Ribu MT", bobot: 4, target: "910,0", realisasi: "991,0", pct: 108.9 },
  { kategori: "B", nama: "Implementasi platform ICO tahap I", satuan: "Waktu", bobot: 8, target: "Go live 30 Jun 2026", realisasi: "Selesai", pct: 110.0 },
  { kategori: "B", nama: "Milestone kewajiban tambang ke negara", satuan: "%", bobot: 15, target: "100", realisasi: "100", pct: 110.0 },
  { kategori: "B", nama: "Feasibility study & AMDAL", satuan: "%", bobot: 8, target: "100", realisasi: "100", pct: 100.0 },
  { kategori: "B", nama: "Kajian program pengembangan batubara", satuan: "Dokumen", bobot: 7, target: "100", realisasi: "100", pct: 100.0 },
  { kategori: "B", nama: "Good Corporate Governance (GCG)", satuan: "%", bobot: 2, target: "100", realisasi: "100", pct: 100.0 },
  { kategori: "B", nama: "Roadmap manajemen risiko", satuan: "%", bobot: 2, target: "100", realisasi: "100,6", pct: 100.6 },
  { kategori: "B", nama: "Maturity level kepatuhan", satuan: "Level", bobot: 2, target: "4,4", realisasi: "4,56", pct: 106.0 },
  { kategori: "B", nama: "Ketepatan waktu & akurasi laporan", satuan: "%", bobot: 4, target: "100", realisasi: "100", pct: 100.0 },
];

/* Detail bulanan per indikator: target, realisasi, capaian (%) — Jan s.d. Jul 2026 */
const monthlyDetail = {
  "Pendapatan service fee": {
    satuan: "Rp Miliar (kumulatif)",
    rows: [
      { bulan: "Jan", target: "49,26", realisasi: "42,94", pct: 87.2 },
      { bulan: "Feb", target: "98,52", realisasi: "94,68", pct: 96.1 },
      { bulan: "Mar", target: "147,77", realisasi: "146,71", pct: 99.3 },
      { bulan: "Apr", target: "197,03", realisasi: "202,49", pct: 102.8 },
      { bulan: "Mei", target: "246,29", realisasi: "261,05", pct: 106.0 },
      { bulan: "Jun", target: "295,55", realisasi: "332,11", pct: 112.4 },
      { bulan: "Jul", target: "379,42", realisasi: "398,56", pct: 105.0 },
    ],
  },
  "Pengendalian anggaran operasi": {
    satuan: "% penyerapan (kumulatif) — makin rendah makin baik",
    rows: [
      { bulan: "Jan", target: "8,0", realisasi: "2,7", pct: 110.0 },
      { bulan: "Feb", target: "17,0", realisasi: "3,3", pct: 110.0 },
      { bulan: "Mar", target: "25,0", realisasi: "4,4", pct: 110.0 },
      { bulan: "Apr", target: "33,0", realisasi: "5,0", pct: 110.0 },
      { bulan: "Mei", target: "42,0", realisasi: "5,3", pct: 110.0 },
      { bulan: "Jun", target: "50,0", realisasi: "11,0", pct: 177.9 },
      { bulan: "Jul", target: "58,0", realisasi: "15,2", pct: 110.0 },
    ],
  },
  "Pendapatan inovatif": {
    satuan: "Rp Miliar (kumulatif)",
    rows: [
      { bulan: "Jan", target: "190,00", realisasi: "192,31", pct: 101.2 },
      { bulan: "Feb", target: "821,46", realisasi: "681,11", pct: 100.0 },
      { bulan: "Mar", target: "1.097,08", realisasi: "1.099,65", pct: 100.0 },
      { bulan: "Apr", target: "1.712,92", realisasi: "1.743,55", pct: 101.8 },
      { bulan: "Mei", target: "2.178,65", realisasi: "2.557,76", pct: 117.4 },
      { bulan: "Jun", target: "2.414,40", realisasi: "2.972,04", pct: 123.1 },
      { bulan: "Jul", target: "3.268,00", realisasi: "4.056,68", pct: 110.0 },
    ],
  },
  "Efisiensi pengelolaan energi primer": {
    satuan: "Rp Miliar (kumulatif)",
    rows: [
      { bulan: "Jan", target: "0,09", realisasi: "0,09", pct: 100.9 },
      { bulan: "Feb", target: "6,42", realisasi: "9,83", pct: 153.1 },
      { bulan: "Mar", target: "9,63", realisasi: "10,88", pct: 110.0 },
      { bulan: "Apr", target: "13,03", realisasi: "13,03", pct: 100.0 },
      { bulan: "Mei", target: "13,18", realisasi: "13,18", pct: 100.0 },
      { bulan: "Jun", target: "19,50", realisasi: "23,35", pct: 119.7 },
      { bulan: "Jul", target: "21,88", realisasi: "28,49", pct: 130.2 },
    ],
  },
  "Pasokan batubara — tambang sendiri & afiliasi": {
    satuan: "Ribu MT (kumulatif)",
    rows: [
      { bulan: "Jan", target: "52,5", realisasi: "70,5", pct: 134.3 },
      { bulan: "Feb", target: "97,5", realisasi: "172,7", pct: 177.1 },
      { bulan: "Mar", target: "142,5", realisasi: "297,8", pct: 209.0 },
      { bulan: "Apr", target: "187,5", realisasi: "377,8", pct: 201.5 },
      { bulan: "Mei", target: "257,5", realisasi: "427,8", pct: 166.2 },
      { bulan: "Jun", target: "327,5", realisasi: "488,1", pct: 149.0 },
      { bulan: "Jul", target: "467,5", realisasi: "541,6", pct: 110.0 },
    ],
  },
  "Pasokan batubara — ke Coal Blending Facility": {
    satuan: "Ribu MT (kumulatif)",
    rows: [
      { bulan: "Jan", target: "30,0", realisasi: "70,0", pct: 233.3 },
      { bulan: "Feb", target: "80,0", realisasi: "125,0", pct: 156.3 },
      { bulan: "Mar", target: "100,0", realisasi: "125,0", pct: 125.0 },
      { bulan: "Apr", target: "125,0", realisasi: "170,0", pct: 136.0 },
      { bulan: "Mei", target: "200,0", realisasi: "240,0", pct: 120.0 },
      { bulan: "Jun", target: "270,0", realisasi: "290,0", pct: 107.4 },
      { bulan: "Jul", target: "350,0", realisasi: "359,5", pct: 102.7 },
    ],
  },
  "Pasokan batubara — ke Intermediate Stockpile": {
    satuan: "Ribu MT (kumulatif)",
    rows: [
      { bulan: "Jan", target: "90,0", realisasi: "101,3", pct: 112.5 },
      { bulan: "Feb", target: "90,0", realisasi: "238,8", pct: 101.6 },
      { bulan: "Mar", target: "235,0", realisasi: "388,9", pct: 99.7 },
      { bulan: "Apr", target: "500,0", realisasi: "550,5", pct: 110.1 },
      { bulan: "Mei", target: "610,0", realisasi: "701,4", pct: 115.0 },
      { bulan: "Jun", target: "780,0", realisasi: "842,1", pct: 108.0 },
      { bulan: "Jul", target: "910,0", realisasi: "991,0", pct: 108.9 },
    ],
  },
  "Implementasi platform ICO tahap I": {
    satuan: "Status penyelesaian",
    rows: [
      { bulan: "Jan", target: "—", realisasi: "Belum dimulai", pct: null },
      { bulan: "Feb", target: "—", realisasi: "Belum dimulai", pct: null },
      { bulan: "Mar", target: "—", realisasi: "Belum dimulai", pct: null },
      { bulan: "Apr", target: "—", realisasi: "Belum dimulai", pct: null },
      { bulan: "Mei", target: "—", realisasi: "Belum dimulai", pct: null },
      { bulan: "Jun", target: "Go live 30 Jun 2026", realisasi: "Selesai (go live)", pct: 110.0 },
      { bulan: "Jul", target: "—", realisasi: "Selesai", pct: 110.0 },
    ],
  },
  "Milestone kewajiban tambang ke negara": {
    satuan: "% (tidak kena sanksi penghentian operasi)",
    rows: [
      { bulan: "Jan", target: "100", realisasi: "Tidak ada sanksi", pct: 100.0 },
      { bulan: "Feb", target: "100", realisasi: "Tidak ada sanksi", pct: 100.0 },
      { bulan: "Mar", target: "100", realisasi: "Tidak ada sanksi", pct: 100.0 },
      { bulan: "Apr", target: "100", realisasi: "Tidak ada sanksi", pct: 100.0 },
      { bulan: "Mei", target: "100", realisasi: "Tidak ada sanksi", pct: 100.0 },
      { bulan: "Jun", target: "100", realisasi: "100", pct: 100.0 },
      { bulan: "Jul", target: "100", realisasi: "110", pct: 110.0 },
    ],
  },
  "Feasibility study & AMDAL": {
    satuan: "% penyelesaian",
    rows: [
      { bulan: "Jan", target: "—", realisasi: "Belum jatuh tempo", pct: null },
      { bulan: "Feb", target: "—", realisasi: "Belum jatuh tempo", pct: null },
      { bulan: "Mar", target: "—", realisasi: "Belum jatuh tempo", pct: null },
      { bulan: "Apr", target: "—", realisasi: "Belum jatuh tempo", pct: null },
      { bulan: "Mei", target: "—", realisasi: "Belum jatuh tempo", pct: null },
      { bulan: "Jun", target: "100", realisasi: "100", pct: 100.0 },
      { bulan: "Jul", target: "100", realisasi: "100", pct: 100.0 },
    ],
  },
  "Kajian program pengembangan batubara": {
    satuan: "Dokumen",
    rows: [
      { bulan: "Jan", target: "0", realisasi: "0", pct: null },
      { bulan: "Feb", target: "—", realisasi: "—", pct: null },
      { bulan: "Mar", target: "—", realisasi: "—", pct: null },
      { bulan: "Apr", target: "—", realisasi: "—", pct: null },
      { bulan: "Mei", target: "—", realisasi: "—", pct: null },
      { bulan: "Jun", target: "100", realisasi: "100", pct: 100.0 },
      { bulan: "Jul", target: "100", realisasi: "100", pct: 100.0 },
    ],
  },
  "Good Corporate Governance (GCG)": {
    satuan: "% penyelesaian program kerja",
    rows: [
      { bulan: "Jan", target: "100", realisasi: "0", pct: 0 },
      { bulan: "Feb", target: "100", realisasi: "0", pct: 0 },
      { bulan: "Mar", target: "100", realisasi: "0", pct: 0 },
      { bulan: "Apr", target: "100", realisasi: "0", pct: 0 },
      { bulan: "Mei", target: "100", realisasi: "—", pct: null },
      { bulan: "Jun", target: "100", realisasi: "100", pct: 100.0 },
      { bulan: "Jul", target: "100", realisasi: "100", pct: 100.0 },
    ],
  },
  "Roadmap manajemen risiko": {
    satuan: "% realisasi program",
    rows: [
      { bulan: "Jan", target: "100", realisasi: "100", pct: 100.0 },
      { bulan: "Feb", target: "100", realisasi: "100", pct: 100.0 },
      { bulan: "Mar", target: "100", realisasi: "100", pct: 100.0 },
      { bulan: "Apr", target: "100", realisasi: "100", pct: 100.0 },
      { bulan: "Mei", target: "100", realisasi: "100", pct: 100.0 },
      { bulan: "Jun", target: "100", realisasi: "100", pct: 100.0 },
      { bulan: "Jul", target: "100", realisasi: "100,6", pct: 100.6 },
    ],
  },
  "Maturity level kepatuhan": {
    satuan: "Level (skala kematangan)",
    rows: [
      { bulan: "Jan", target: "—", realisasi: "0", pct: 0 },
      { bulan: "Feb", target: "—", realisasi: "0", pct: 0 },
      { bulan: "Mar", target: "—", realisasi: "0", pct: 0 },
      { bulan: "Apr", target: "—", realisasi: "0", pct: 0 },
      { bulan: "Mei", target: "—", realisasi: "—", pct: null },
      { bulan: "Jun", target: "4,3", realisasi: "4,56", pct: 106.0 },
      { bulan: "Jul", target: "—", realisasi: "4,56", pct: 106.0 },
    ],
  },
  "Ketepatan waktu & akurasi laporan": {
    satuan: "% ketepatan waktu",
    rows: [
      { bulan: "Jan", target: "100", realisasi: "100", pct: 100.0 },
      { bulan: "Feb", target: "100", realisasi: "100", pct: 100.0 },
      { bulan: "Mar", target: "100", realisasi: "110", pct: 110.0 },
      { bulan: "Apr", target: "100", realisasi: "110", pct: 110.0 },
      { bulan: "Mei", target: "100", realisasi: "110", pct: 110.0 },
      { bulan: "Jun", target: "100", realisasi: "100", pct: 100.0 },
      { bulan: "Jul", target: "100", realisasi: "100", pct: 100.0 },
    ],
  },
};

const komposisiB = [
  { nama: "Pasokan batubara", nilai: 12, color: "#7A2E1E" },
  { nama: "Platform ICO", nilai: 8, color: "#C1502E" },
  { nama: "Milestone tambang", nilai: 15, color: "#E28B5D" },
  { nama: "Dokumen penunjang", nilai: 15, color: "#F2C4A6" },
  { nama: "Tata kelola & kepatuhan", nilai: 10, color: "#F8DEC7" },
];

const komposisiA = [
  { nama: "Service fee", nilai: 10, color: "#4B4B4B" },
  { nama: "Anggaran operasi", nilai: 10, color: "#7A7A7A" },
  { nama: "Pendapatan inovatif", nilai: 10, color: "#A6A6A6" },
  { nama: "Efisiensi energi primer", nilai: 10, color: "#D0D0D0" },
];

function statusColor(pct) {
  if (pct >= 105) return { fg: "#0F6E56", bg: "#E1F5EE" };
  if (pct >= 100) return { fg: "#854F0B", bg: "#FAEEDA" };
  return { fg: "#993C1D", bg: "#FAECE7" };
}

function MetricBlock({ icon: Icon, label, value, sub, color }) {
  return (
    <div
      style={{
        background: color,
        borderRadius: 6,
        padding: "16px 12px 14px",
        display: "flex",
        flexDirection: "column",
        alignItems: "center",
        textAlign: "center",
        gap: 8,
        minWidth: 0,
      }}
    >
      <span style={{ fontSize: 10.5, fontWeight: 600, letterSpacing: 0.6, color: "rgba(255,255,255,0.85)" }}>
        {label.toUpperCase()}
      </span>
      <Icon size={26} color="#FFFFFF" strokeWidth={1.4} />
      <span
        style={{
          fontFamily: "'JetBrains Mono', monospace",
          fontSize: 17,
          fontWeight: 600,
          color: "#fff",
          whiteSpace: "nowrap",
        }}
      >
        {value}
      </span>
      <span style={{ fontSize: 10.5, color: "rgba(255,255,255,0.75)" }}>{sub}</span>
    </div>
  );
}

function TrendCard({ title, data, unit }) {
  return (
    <div style={{ background: "#fff", border: `1px solid ${border}`, borderRadius: 8, padding: "16px 18px" }}>
      <div style={{ fontSize: 12.5, fontWeight: 600, color: ink, letterSpacing: 0.3, marginBottom: 2 }}>
        {title.toUpperCase()}
      </div>
      <div style={{ fontSize: 11, color: inkSoft, marginBottom: 10 }}>kumulatif, {unit} — Jan s.d. Jul 2026</div>
      <div style={{ height: 160 }}>
        <ResponsiveContainer width="100%" height="100%">
          <LineChart data={data} margin={{ top: 4, right: 8, left: -22, bottom: 0 }}>
            <CartesianGrid stroke={border} vertical={false} />
            <XAxis dataKey="bulan" tick={{ fontSize: 10, fill: inkSoft }} axisLine={{ stroke: border }} tickLine={false} />
            <YAxis tick={{ fontSize: 10, fill: inkSoft }} axisLine={false} tickLine={false} />
            <Tooltip contentStyle={{ borderRadius: 8, border: `1px solid ${border}`, fontSize: 11 }} />
            <Line type="monotone" dataKey="target" name="Target" stroke="#B4AFA0" strokeWidth={2} strokeDasharray="4 3" dot={false} />
            <Line type="monotone" dataKey="realisasi" name="Realisasi" stroke="#2F6F4E" strokeWidth={2} dot={{ r: 3, fill: "#2F6F4E" }} />
          </LineChart>
        </ResponsiveContainer>
      </div>
      <div style={{ display: "flex", gap: 14, marginTop: 4, fontSize: 10.5, color: inkSoft }}>
        <span style={{ display: "flex", alignItems: "center", gap: 4 }}>
          <span style={{ width: 14, height: 2, background: "#B4AFA0" }} /> target
        </span>
        <span style={{ display: "flex", alignItems: "center", gap: 4 }}>
          <span style={{ width: 14, height: 2, background: "#2F6F4E" }} /> realisasi
        </span>
      </div>
    </div>
  );
}

function DonutCard({ title, data }) {
  return (
    <div style={{ background: "#fff", border: `1px solid ${border}`, borderRadius: 8, padding: "16px 18px" }}>
      <div style={{ fontSize: 12.5, fontWeight: 600, color: ink, letterSpacing: 0.3, marginBottom: 10 }}>
        {title.toUpperCase()}
      </div>
      <div style={{ display: "flex", alignItems: "center", justifyContent: "center" }}>
        <div style={{ width: 120, height: 120, flexShrink: 0 }}>
          <ResponsiveContainer width="100%" height="100%">
            <PieChart>
              <Pie data={data} dataKey="nilai" nameKey="nama" innerRadius={32} outerRadius={58} paddingAngle={1} stroke="none">
                {data.map((d, i) => (
                  <Cell key={i} fill={d.color} />
                ))}
              </Pie>
              <Tooltip contentStyle={{ borderRadius: 8, border: `1px solid ${border}`, fontSize: 12 }} formatter={(v, n) => [`bobot ${v}`, n]} />
            </PieChart>
          </ResponsiveContainer>
        </div>
        <div style={{ display: "flex", flexDirection: "column", gap: 6, marginLeft: 12, justifyContent: "center" }}>
          {data.map((it) => (
            <div key={it.nama} style={{ display: "flex", alignItems: "center", gap: 6, fontSize: 11.5, color: inkSoft }}>
              <span style={{ width: 9, height: 9, background: it.color, borderRadius: 2, flexShrink: 0 }} />
              {it.nama} ({it.nilai})
            </div>
          ))}
        </div>
      </div>
    </div>
  );
}

function MonthlyDetailCard() {
  const namaIndikator = Object.keys(monthlyDetail);
  const [pilihan, setPilihan] = useState(namaIndikator[0]);
  const detail = monthlyDetail[pilihan];
  const chartData = detail.rows.map((r) => ({ bulan: r.bulan, pct: r.pct }));

  return (
    <div style={{ background: "#fff", border: `1px solid ${border}`, borderRadius: 8, padding: "16px 18px", marginBottom: 14 }}>
      <div style={{ display: "flex", justifyContent: "space-between", alignItems: "center", marginBottom: 4, flexWrap: "wrap", gap: 8 }}>
        <div style={{ fontSize: 12.5, fontWeight: 600, color: ink, letterSpacing: 0.3 }}>
          PENCAPAIAN BULANAN PER INDIKATOR
        </div>
        <select
          value={pilihan}
          onChange={(e) => setPilihan(e.target.value)}
          style={{
            border: `1px solid ${border}`,
            borderRadius: 6,
            padding: "6px 10px",
            fontSize: 12.5,
            color: ink,
            background: "#fff",
            maxWidth: 340,
          }}
        >
          {namaIndikator.map((n) => (
            <option key={n} value={n}>
              {n}
            </option>
          ))}
        </select>
      </div>
      <div style={{ fontSize: 11, color: inkSoft, marginBottom: 14 }}>{detail.satuan}</div>

      <div style={{ display: "grid", gridTemplateColumns: "1.3fr 1fr", gap: 18 }}>
        <table style={{ width: "100%", borderCollapse: "collapse", fontSize: 12.5 }}>
          <thead>
            <tr style={{ color: inkSoft, textAlign: "left" }}>
              <th style={{ fontWeight: 500, padding: "0 8px 8px 0" }}>Bulan</th>
              <th style={{ fontWeight: 500, padding: "0 8px 8px 0", textAlign: "right" }}>Target</th>
              <th style={{ fontWeight: 500, padding: "0 8px 8px 0", textAlign: "right" }}>Realisasi</th>
              <th style={{ fontWeight: 500, padding: "0 0 8px 0", textAlign: "right" }}>Capaian</th>
            </tr>
          </thead>
          <tbody>
            {detail.rows.map((r) => {
              const sc = r.pct === null ? { fg: inkSoft, bg: "#F4F2EC" } : statusColor(r.pct);
              return (
                <tr key={r.bulan} style={{ borderTop: `1px solid ${border}` }}>
                  <td style={{ padding: "7px 8px 7px 0", fontWeight: 500 }}>{r.bulan}</td>
                  <td style={{ padding: "7px 8px 7px 0", textAlign: "right", fontFamily: "'JetBrains Mono', monospace" }}>{r.target}</td>
                  <td style={{ padding: "7px 8px 7px 0", textAlign: "right", fontFamily: "'JetBrains Mono', monospace" }}>{r.realisasi}</td>
                  <td style={{ padding: "7px 0", textAlign: "right" }}>
                    <span
                      style={{
                        fontSize: 11,
                        fontWeight: 600,
                        padding: "2px 8px",
                        borderRadius: 5,
                        color: sc.fg,
                        background: sc.bg,
                        fontFamily: "'JetBrains Mono', monospace",
                      }}
                    >
                      {r.pct === null ? "—" : `${r.pct.toFixed(1)}%`}
                    </span>
                  </td>
                </tr>
              );
            })}
          </tbody>
        </table>

        <div>
          <div style={{ fontSize: 11, color: inkSoft, marginBottom: 8 }}>Tren capaian (%) per bulan</div>
          <div style={{ height: 200 }}>
            <ResponsiveContainer width="100%" height="100%">
              <LineChart data={chartData} margin={{ top: 4, right: 8, left: -16, bottom: 0 }}>
                <CartesianGrid stroke={border} vertical={false} />
                <XAxis dataKey="bulan" tick={{ fontSize: 10, fill: inkSoft }} axisLine={{ stroke: border }} tickLine={false} />
                <YAxis tick={{ fontSize: 10, fill: inkSoft }} axisLine={false} tickLine={false} unit="%" />
                <Tooltip contentStyle={{ borderRadius: 8, border: `1px solid ${border}`, fontSize: 11 }} formatter={(v) => [`${v}%`, "Capaian"]} />
                <Line type="monotone" dataKey="pct" stroke="#2F6F4E" strokeWidth={2} dot={{ r: 3, fill: "#2F6F4E" }} connectNulls />
              </LineChart>
            </ResponsiveContainer>
          </div>
        </div>
      </div>
    </div>
  );
}

export default function Dashboard() {
  const [kategori, setKategori] = useState("Semua");
  const filtered = indikator.filter((d) => kategori === "Semua" || d.kategori === kategori);

  return (
    <div style={{ background: "#EFEDE6", minHeight: "100vh", fontFamily: "'Inter', sans-serif", padding: "24px 22px 50px" }}>
      <link
        rel="stylesheet"
        href="https://fonts.googleapis.com/css2?family=Fraunces:opsz,wght@9..144,700&family=Inter:wght@400;500;600&family=JetBrains+Mono:wght@500;600&display=swap"
      />

      <div style={{ maxWidth: 1120, margin: "0 auto" }}>
        <div style={{ marginBottom: 20 }}>
          <div style={{ fontSize: 11.5, letterSpacing: 1.2, color: inkSoft, marginBottom: 4 }}>
            PT PLN ENERGI PRIMER INDONESIA — SVP PENGEMBANGAN USAHA BATUBARA
          </div>
          <h1
            style={{
              fontFamily: "'Fraunces', serif",
              fontWeight: 700,
              fontSize: 25,
              margin: 0,
              color: "#3B4A9E",
            }}
          >
            REALISASI KONTRAK MANAJEMEN 2026 — S.D. JULI
          </h1>
        </div>

        {/* Metric blocks */}
        <div style={{ display: "grid", gridTemplateColumns: "repeat(6, 1fr)", gap: 4, marginBottom: 22 }}>
          {metricBlocks.map((m) => (
            <MetricBlock key={m.label} {...m} />
          ))}
        </div>

        {/* Trend charts */}
        <div style={{ display: "grid", gridTemplateColumns: "1fr 1fr 1fr", gap: 12, marginBottom: 14 }}>
          <TrendCard title="Pendapatan service fee" data={serviceFee} unit="Rp Miliar" />
          <TrendCard title="Pendapatan inovatif" data={pendapatanInovatif} unit="Rp Miliar" />
          <TrendCard title="Efisiensi energi primer" data={efisiensiEnergi} unit="Rp Miliar" />
        </div>

        {/* Donut composition */}
        <div style={{ display: "grid", gridTemplateColumns: "1fr 1fr", gap: 14, marginBottom: 14 }}>
          <DonutCard title="Komposisi bobot kategori KPI (A · total 40)" data={komposisiA} />
          <DonutCard title="Komposisi bobot performance indicators (B · total 60)" data={komposisiB} />
        </div>

        {/* Detail bulanan per indikator */}
        <MonthlyDetailCard />

        {/* Table */}
        <div style={{ background: "#fff", border: `1px solid ${border}`, borderRadius: 8, padding: "16px 18px" }}>
          <div style={{ display: "flex", justifyContent: "space-between", alignItems: "center", marginBottom: 12, flexWrap: "wrap", gap: 8 }}>
            <div style={{ fontSize: 12.5, fontWeight: 600, color: ink, letterSpacing: 0.3 }}>
              RINCIAN INDIKATOR KINERJA — REALISASI S.D. JULI 2026
            </div>
            <div style={{ display: "flex", gap: 6, background: "#F4F2EC", borderRadius: 8, padding: 4 }}>
              {["Semua", "A", "B"].map((k) => (
                <button
                  key={k}
                  onClick={() => setKategori(k)}
                  style={{
                    border: "none",
                    cursor: "pointer",
                    padding: "5px 12px",
                    borderRadius: 6,
                    fontSize: 12,
                    fontWeight: 500,
                    background: kategori === k ? ink : "transparent",
                    color: kategori === k ? "#fff" : inkSoft,
                  }}
                >
                  {k === "Semua" ? "Semua" : `Kategori ${k}`}
                </button>
              ))}
            </div>
          </div>
          <table style={{ width: "100%", borderCollapse: "collapse", fontSize: 12.5 }}>
            <thead>
              <tr style={{ color: inkSoft, textAlign: "left" }}>
                <th style={{ fontWeight: 500, padding: "0 8px 8px 0" }}>Indikator</th>
                <th style={{ fontWeight: 500, padding: "0 8px 8px 0" }}>Satuan</th>
                <th style={{ fontWeight: 500, padding: "0 8px 8px 0", textAlign: "right" }}>Bobot</th>
                <th style={{ fontWeight: 500, padding: "0 8px 8px 0", textAlign: "right" }}>Target</th>
                <th style={{ fontWeight: 500, padding: "0 8px 8px 0", textAlign: "right" }}>Realisasi</th>
                <th style={{ fontWeight: 500, padding: "0 0 8px 0", textAlign: "right" }}>Capaian</th>
              </tr>
            </thead>
            <tbody>
              {filtered.map((d, i) => {
                const sc = statusColor(d.pct);
                return (
                  <tr key={i} style={{ borderTop: `1px solid ${border}` }}>
                    <td style={{ padding: "8px 8px 8px 0" }}>{d.nama}</td>
                    <td style={{ padding: "8px 8px 8px 0", color: inkSoft }}>{d.satuan}</td>
                    <td style={{ padding: "8px 8px 8px 0", textAlign: "right", fontFamily: "'JetBrains Mono', monospace" }}>{d.bobot}</td>
                    <td style={{ padding: "8px 8px 8px 0", textAlign: "right", fontFamily: "'JetBrains Mono', monospace" }}>{d.target}</td>
                    <td style={{ padding: "8px 8px 8px 0", textAlign: "right", fontFamily: "'JetBrains Mono', monospace" }}>{d.realisasi}</td>
                    <td style={{ padding: "8px 0", textAlign: "right" }}>
                      <span
                        style={{
                          fontSize: 11,
                          fontWeight: 600,
                          padding: "2px 8px",
                          borderRadius: 5,
                          color: sc.fg,
                          background: sc.bg,
                          fontFamily: "'JetBrains Mono', monospace",
                        }}
                      >
                        {d.pct.toFixed(1)}%
                      </span>
                    </td>
                  </tr>
                );
              })}
            </tbody>
          </table>
        </div>

        <div style={{ marginTop: 18, fontSize: 11, color: inkSoft, textAlign: "center" }}>
          Sumber: berkas "REALISASI USULAN KONTRAK MANAJEMEN TAHUN 2026" — realisasi s.d. Juli 2026, Jakarta 5 Agustus 2026.
          Catatan: pada indikator Pengendalian Anggaran Operasi, capaian dihitung berdasarkan efisiensi penyerapan anggaran (penyerapan rendah = capaian tinggi).
        </div>
      </div>
    </div>
  );
}
