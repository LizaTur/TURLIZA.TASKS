Проверка, является ли число простым

function isprime_(n::T)::Bool where T <: Integer
for i in 2:round(T, sqrt(n))
if n % i == 0
return false
end
end
return true
end
