Teste
#####
:date: 2009-04-15 12:46
:author: ispmarin
:category: rede, segurança
:tags: net, security, segurança
:slug: teste
:status: published

O cara que descobriu o DNS Poisoning (lembrando que não sabemos o que
está acontecendo no servidor DNS do Virtua, pode ser isso ou não!!), Dan
Kamdinsky, tem um teste para um server DNS, sobre a aleatoriedade das
portas de resposta. Testem com

dig +short @\ `201.6.0.43 <http://201.6.0.43/>`__
`porttest.dns-oarc.net <http://porttest.dns-oarc.net/>`__ TXT

e veja se o resultado é o quê. Postem aqui para discutirmos.

O Rafael acabou de testar o server do Virtua:

`porttest.y.x.w.v.u.t.s.r.q.p.o.n.m.l.k.j.i.h.g.f.e.d.c.b.a.pt.dns-oarc.net <http://porttest.y.x.w.v.u.t.s.r.q.p.o.n.m.l.k.j.i.h.g.f.e.d.c.b.a.pt.dns-oarc.net/>`__.
 "201.6.0.43 is GREAT: 26 queries in 4.8 seconds from 26 ports with std
dev 20760"

Ou seja, parece que a aleatoriedade das portas deste servidor é boa.
Mais investigação é necessária. Assim que tiver tempo junto mais
informações sobre esse teste.
