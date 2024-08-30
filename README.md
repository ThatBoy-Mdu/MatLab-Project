# MatLab-Project

```MatLab
% MATLAB code to simulate the transient response of an RC circuit

% Circuit parameters
R = 1000;         % Resistance in ohms
C = 10e-6;        % Capacitance in farads
V_in = 5;         % Input voltage in volts

% Time vector (0 to 0.1 seconds with a step of 1 ms)
t = 0:1e-4:0.1;

% Calculate the voltage across the capacitor V_C(t)
V_C = V_in * (1 - exp(-t / (R * C)));

% Plot the results
figure;
plot(t, V_C, 'r-', 'LineWidth', 2);
title('Transient Response of an RC Circuit');
xlabel('Time (s)');
ylabel('Voltage across Capacitor V_C(t) (V)');
grid on;

% Display the plot
hold off;
```
![Figure 1 MatLab](https://github.com/user-attachments/assets/53d38222-aec6-4e8a-a9f4-b13ec52cc082)


