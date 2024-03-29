---
description: Виртуализация в Linux
cover: >-
  https://images.unsplash.com/flagged/photo-1579274216947-86eaa4b00475?crop=entropy&cs=srgb&fm=jpg&ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHw0fHxzZXJ2ZXJ8ZW58MHx8fHwxNzA3MDExMDc3fDA&ixlib=rb-4.0.3&q=85
coverY: 0
---

# 🧬 Виртуализация

## QUEMU

**QEMU** (Quick Emulator) — бесплатный эмулятор с открытым исходным кодом . Он эмулирует процессор компьютера посредством динамической двоичной трансляции и предоставляет для машины набор различных моделей аппаратного обеспечения и устройств, что позволяет ей запускать различные гостевые операционные системы. Он может взаимодействовать с виртуальной машиной на основе ядра (KVM) для запуска виртуальных машин с производительностью близкой к исходной. QEMU также может эмулировать процессы пользовательского уровня, позволяя приложениям, скомпилированным для одной архитектуры, работать на другой.

QEMU поддерживает эмуляцию различных архитектур, включая x86, ARM, PowerPC, RISC-V и других.

## KVM

KVM (Kernel-based Virtual Machine) — это бесплатный модуль виртуализации с открытым исходным кодом в ядре Linux, который позволяет ядру функционировать в качестве гипервизора. Он был объединен с основным ядром Linux в версии 2.6.20, выпущенной 5 февраля 2007 года. Для KVM требуется процессор с расширениями аппаратной виртуализации, такими как Intel VT или AMD-V. KVM также был портирован на другие операционные системы, такие как FreeBSD и illumos в виде загружаемых модулей ядра.

KVM поддерживает аппаратную виртуализацию для широкого спектра гостевых операционных систем, включая BSD, Solaris, Windows, Haiku, ReactOS, Plan 9, AROS, macOS и даже другие системы Linux. Кроме того, Android 2.2, GNU/Hurd (Debian K16), Minix 3.1.2a, Solaris 10 U3 и Darwin 8.0.1, а также другие операционные системы и некоторые более новые версии из перечисленных, известно, что они работают с определенными ограничениями.

Кроме того, KVM обеспечивает поддержку паравиртуализации для Linux, OpenBSD, FreeBSD, NetBSD, Plan 9 и гостей Windows с использованием API VirtIO. Сюда входит паравиртуальная карта Ethernet, дисковый контроллер I/O, драйвер balloon и графический интерфейс VGA с использованием драйверов SPICE или VMware.

## libvirt

libvirt — это API с открытым исходным кодом, демон и инструмент для управления виртуализацией платформы. Его можно использовать для управления KVM, Xen, VMware ESXi, QEMU и другими технологиями виртуализации. Эти API широко используются на уровне оркестрации гипервизоров при разработке облачных решений.
