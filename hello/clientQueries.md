query getAllUsers
{users{id,firstname}}

---

query getQuotes{
quotes{
name,by
}
}

---

query getUserById{
  user(id:"12222"){
    id
    firstname
    lastname
    email
    quotes{
      name
    }
  }
}

--
query getQuoteByUser{
  iquote(by:"12222"){
    name
    by
  }
}